## Component Name

Output Process Result

## Primary Language

日本語

## Summary

ロボットのプロセス実行結果をHTMLに出力します。
1回の実行が1ファイルになるため、確認が容易になります。
ブラウザ表示したまま実行終了すれば「終わったかどうか・結果はどうだったか」を後から確認する事もできます。

## Description

このワークフローを呼び出すと、実行時にログに出力した内容、及び実行環境をHTMLファイルで作成します。
HTMLファイルをブラウザで画面に表示し、実行結果として確認することも出来ます。

ワークフローの引数は下記になります。
In_LogDirectory：実行ログファイルのディレクトリパス（未指定時はデフォルト保存先パス）
In_OutputDirectory：HTMLの出力先ディレクトリパス　例：Result（プロジェクト直下のResultフォルダ）
In_OpenWithBrowser：HTMLをブラウザで表示するか（True：表示する）

HTMLファイルに出力される内容は下記になります。

ProjectName：プロジェクト名
ProjectDescription：プロジェクト説明
MachineName：マシン名
UserName：ユーザー名
CurrentDateTime：現在日時
ProcessLog：実行ログ

## Benefits

ロボットのプロセス実行結果の確認・把握がしやすくなります。

## Process/Industry

金融 & 財務 法務 人事 IT 営業 & 販売

## Tags

## Compatibility

UiPath Studio 2018.4.5, UiPath Studio 2019.4 UiPath Studio 2019.12 で動作確認済み

## Dependencies

依存なし

## Media

<img src="/OutputProcessLogToHtml/images/argument.png" alt=""><br>
<img src="/OutputProcessLogToHtml/images/html.png" alt=""><br>
<img src="/OutputProcessLogToHtml/images/workflow.png" alt="">
