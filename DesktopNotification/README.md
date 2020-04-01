
営業日取得

## Component Name

DesktopNotificationWithXaml

## Primary Language

日本語

## Summary

下記カスタムアクティビティのXamlファイル版です。

https://connect.uipath.com/ja/marketplace/components/desktop-notification
機能的には、ほぼ同じものです。
「プロジェクトの都合により、カスタムアクティビティの採用は難しいが、XAMLであれば（コード確認できるので）採用しても問題ない」という場合はこちらを使用下さい。


## Benefits

現在実行中の内容を画面に表示し、伝えることが出来ます。

## Description

デスクトップ右下にメッセージウィンドウを表示します。
表示されたウィンドウはプロジェクトファイルの実行終了とともに自動的に消滅します。
以下の3ファイルでウィンドウを操作します。

- ShowNotification.xaml（デスクトップ右下に「通知ウィンドウ」を表示）
- ShowProgressNotification.xaml（デスクトップ右下に「進捗率付きの通知ウィンドウ」を表示）
- CloseNotification.xaml（デスクトップに表示した「通知ウィンドウ」を消す）

背景色や文字サイズ等のデザインは、InvokeCode内のコードを変えればカスタマイズできます。

ShowNotification.xaml は下記のように呼び出します。

- 引数1）［in_Title］"タイトルとして表示する文字列"
- 引数2）［in_Message］"メッセージとして表示する文字列"


ShowProgressNotification.xaml は下記のように呼び出します。

- 引数1）［in_Title］"タイトルとして表示する文字列"
- 引数2）［in_Message］"メッセージとして表示する文字列"
- 引数3）［in_ProgressRate］進捗率（0-100の数値）



## Process/Industry

金融 & 財務 法務 人事 IT 営業 & 販売

## Tags



## Compatibility

UiPath Studio 2018.4.5, UiPath Studio 2019.4 UiPath Studio 2019.12 で動作確認済み

## Dependencies

依存なし

## Media

