
営業日取得

## Component Name

GetNextBusinessDay

## Primary Language

日本語

## Summary

Excelシートで設定した内容に基づき、N日先（N日前）の営業日を計算します。
設定はシンプルで「曜日別の営業日ルール」「日付別の特別営業日ルール」から構成され、
必要最低限の設定で済むように設計しています。

## Benefits

営業日の計算がシンプルに実現できます。

## Description

営業日の設定に基づき、N日先（N日前）の営業日を計算します。

まず、Excelシートで下記を設定します。

-「曜日ルール」シートに、曜日別の営業設定を入力
  - 営業する曜日は「営業する」と入力します（営業しない曜日＝「営業しない」と入力）	
-「特別日リスト」シートに、日付別の営業設定を入力
  - 曜日ルールに関係なく、営業する（しない）日を入力します
  - 初期データとして、下記3つを設定してあります。
    - 2030年までの祝日を「営業しない」日で設定
    - 2030年までの12月30日、12月31日を「営業しない」日で設定
    - 2030年までの1月1日、1月2日、1月3日を「営業しない」日で設定
  - 必要に応じて変更してください。（例：12/31は曜日関係なく「営業する」日で設定など）	


次に、GetNextBusinessDay.xaml を下記のように呼び出してください。

引数1）［in_Date］CDate("2020/3/26")
引数2）［in_addDate］3
引数3）［in_BusinessDayExcelPath］"C:\temp\営業日設定.xlsx"
引数4）［out_Date］Result

「営業日設定.xlsx」の内容に基づき「2020/3/26（木）」の「3」営業日後の値を計算し、Resultにセットされます

※ 引数2に「マイナスの値」をセットすることで、N日前の営業日も計算できます。





## Process/Industry

金融 & 財務 法務 人事 IT 営業 & 販売

## Tags



## Compatibility

UiPath Studio 2018.4.5, UiPath Studio 2019.4 UiPath Studio 2019.12 で動作確認済み

## Dependencies

依存なし

## Media


## Memo

Excel

・営業日.xlsx

・営業日ルールSheet

　　Header）月曜／火曜営業／・・・／日曜営業／祝日営業

・祝日リストSheet

　　Header）日付／曜日／祝日名

・特別営業日リストSheet

　　Header）日付／備考


引数

- In_baseDate Date 基準日付
- In_addDays Integer 加算減算日数
- Out_resultDate Date 結果日付

処理
- WeekDayValueList = {"月曜","火曜","水曜","木曜","金曜","土曜","日曜","祝日"}


- 各シート読み込み（それぞれDatatableへ）
  - DtBusinessDayRule
    - BusinessDayRuleDict = New Dictionary（Of String,
    - ForEach col In DtBusinessDayRule.Columns
      - ForEach val In WeekDayValueList
        - IF col.contains(val) THEN BusinessDayRuleDict(val) = DtBusinessDayRule(0)(Col) EXIT FOR
  - DtHoliday
    -> HolidayList
  - DtSpecialBusinessDay
    -> SpecialBusinessDayList


- 営業日数計算（加算減算日数の数だけ・プラスマイナス考慮）
- 移動日数初期化
- ループ（営業日数がゼロになるまで）
  - 営業日フラグ初期化
  - ループ（営業日と判定されるまで）
    - 判定１）移動日付が特別営業日か判定
    - 判定２）移動日付の曜日を取得
    - 判定３）該当曜日が営業対象か判定
    - 上記判定１－３で営業日ならループを抜ける


類似コンポーネント


https://connect.uipath.com/ja/marketplace/components/persol-workday-calender-calculate-robot

https://www.rpahiroba.com/2018/07/27/uipath%e3%81%a7%e7%bf%8c%e5%96%b6%e6%a5%ad%e6%97%a5%e3%82%92%e5%8f%96%e5%be%97%e3%81%99%e3%82%8b%e6%96%b9%e6%b3%95/
