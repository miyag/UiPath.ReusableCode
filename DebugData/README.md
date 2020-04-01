## Component Name

DebugData

## Primary Language

日本語

## Summary

データの内容をデバッグ出力します。
値が入っているか？どんな値が入っているかを確認したい時に利用できます。

## Benefits

ワークフロー呼び出しでデータの中身を確認できます。
面倒なループ構文や、難しいLINQ構文を書く必要はありません。
データ数や列定義もデバッグ表示します。
表示するデータ数や列数を指定し、デバッグウィンドウに表示される文字列を減らすことも出来ます。

## Description

デバッグ出力対象の種類別にワークフローが別れています。

1）DebugDataRow.xaml

データ行の内容をデバッグ出力します

引数

- in_DataRow : データ行
- in_DebugColumnsCount : デバッグ表示する「列」数のリミット

出力例

DebugDataRow (Columns.Count=2 [DisplayLimit=10])
[Column] A列 B列 
[Row] 値１ 値２


2）DebugDataTable.xaml

データテーブルの内容をデバッグ出力します

引数

- in_DataTable : データテーブル
- in_DebugRowsCount : デバッグ表示する「行」数のリミット
- in_DebugColumnsCount : デバッグ表示する「列」数のリミット

出力例

DebugDataTable (Rows.Count=2 [DisplayLimit=3], Columns.Count=2 [DisplayLimit=3]
[Column] A列 B列 
[Row-1] 値１１ 値１２ 
[Row-2] 値２１ 値２２


3）DebugDictionary.xaml

ディクショナリ（※）の内容をデバッグ出力します（※ Key=String型、Value=Object型）

引数

- in_Dictionary : ディクショナリ
- in_DebugDataCount : デバッグ表示するデータ数のリミット

出力例

DebugDictionary (Count=3 [DisplayLimit=10])
[キー１] 値１
[キー２] 値２
[キー３] 値３



## Process/Industry

金融 & 財務 法務 人事 IT 営業 & 販売

## Tags

デバッグ

## Compatibility

UiPath Studio 2018.4.5, UiPath Studio 2019.4 UiPath Studio 2019.12 で動作確認済み

## Dependencies

依存なし

## Media
