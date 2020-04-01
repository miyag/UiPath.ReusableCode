
値のチェック

## Component Name

CheckValue

## Primary Language

日本語

## Summary

値のチェックを行うXamlファイルです。

設定ファイルの値や入力値の検証に使用できます。
エラー時は例外をスローします。
エラーメッセージは変更しやすいように各ファイルの先頭で定義してあります。

## Benefits

値のチェックをフロー呼び出しで単純に処理できます。

## Description

チェックの内容別にxamlファイルが別れています。

- CheckValueContains.xaml：文字列がリストに含まれるか？
- CheckValueDate.xaml：日付型か？範囲内の日付か？
- CheckValueDirectoryExists.xaml：ディレクトリが存在するか？
- CheckValueFileExists.xaml：ファイルが存在するか？
- CheckValueFileName.xaml：ファイル名として使用できるか？
- CheckValueLength.xaml：文字列の長さが範囲内か？
- CheckValueMailAddress.xaml：メールアドレス形式が妥当か？
- CheckValueNumeric.xaml：数値型か？範囲内の数値か？
- CheckValueRequired.xaml：値が設定されているか？
- CheckValueSheetExists.xaml：シートが存在するか？
- CheckValueSheetName.xaml：シート名が使用できるか？
- CheckValueUrl.xaml：URLの形式が妥当か？

「必須かつ数字」の値をチェックする場合、
CheckValueRequired.xaml の後で CheckValueNumeric.xaml を呼び出して下さい。

## Process/Industry

金融 & 財務 法務 人事 IT 営業 & 販売

## Tags

## Compatibility

UiPath Studio 2018.4.5, UiPath Studio 2019.4 UiPath Studio 2019.12 で動作確認済み

## Dependencies

依存なし

## Media

