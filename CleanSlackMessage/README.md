# ExportRobotLogToExcel

SlackのAPIを使用して、指定チャンネルのメッセージを削除

## Component Name

CleanSlackMessage

## Primary Language Select

日

## Summary

APIでチャンネル内のメッセージを削除します。
対象メッセージは「日付範囲」「対象ワード/除外ワードを」で絞り込みが可能です。
削除したメッセージはテキストファイルにバックアップとして出力します。

## Benefits

メッセージを一括で削除できます。
条件を指定して絞り込みも可能です。削除したメッセージはファイルにバックアップ出力されます。

## Description

処理の流れ

- 1. 処理で使用するトークンをセット
- 2. メッセージ削除の条件を指定
- 3. APIからメッセージリストを取得（https://slack.com/api/conversations.history）
- 4. 削除条件に合致するメッセージをリストに退避
- 5. 削除実行前の確認表示（ダイアログ表示）
- 6. APIでメッセージを削除（https://slack.com/api/chat.delete）
- 7. 削除件数の表示（メッセージボックス表示）



## Process/Industry

Finance & Accounting Legal Human Resources Information Technology Sales

金融 & 財務 法務 人事 IT 営業 & 販売

## Tags

  
## Compatibility

Tested with UiPath Studio 2020.10.0

UiPath Studio 2020.10.0 で動作確認済み

## Dependencies

No Dependencies

依存なし

## Media

<img src="/CleanSlackMessage/Images/wf.png" alt="">
