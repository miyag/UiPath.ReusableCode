## Component Name

SearchTweets

## Primary Language Select

日

## Summary

Twitterに投稿される情報をAPIを利用して収集します。
指定条件でツィートを検索し、ExcelとHtmlに出力することでファイルで一覧確認できます。

## Benefits

ワークフローの実行で、ツィートの収集が簡単にできます。

## Description

Twitterの検索APIから、指定の条件で取得したデータをExcel及びHtmlに出力します。

検索するために、下記をワークフローで設定します。

- ConsumerKey（APIアクセスで使用するID）
- ConsumerSecret（APIアクセスで使用するパスワード）
- OutputDirectory（結果を出力するフォルダ）
- SearchKeyword（検索キーワード）
- SearchLang（検索する言語。jaの場合は日本のツィートのみが対象）

## Tags

twitter tweet oauth  

## Compatibility

2019.4 UiPath Studio 2019.12 で動作確認済み

Tested with UiPath Studio 2019.4 & 2019.12

## Dependencies

No Dependencies

依存なし

## Media

<img src="/SearchTweet/Images/argument.png" alt=""><br>
<img src="/SearchTweet/Images/workflow.png" alt=""><br>
<img src="/SearchTweet/Images/excel.png" alt=""><br>
<img src="/SearchTweet/Images/html.png" alt="">