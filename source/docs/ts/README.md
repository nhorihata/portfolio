# Aem TypeScript Templates 
gulpでコンパイルして使うTypeScriptファイルテンプレートです。  
gulpからwebpackを使ってトランスパイル、モジュールバンドルをしています。

# version
ver 1.0.0 (2019/1/10)

# 仕様
記述方法などについてのサンプルを`exammple.ts`内に記述しています。  
実際に使う時には削除しちゃってください。

ざっくりと仕様はこんな感じ

* `ES6モジュール`で外部モジュールを使用できます。
* `アンダーバー(_)`始まりのファイルはコンパイルされません。外部モジュールとして使ってください。
* 型定義に困った時は`@types/typing.d.ts`に定義すれば解決できます。
* ソースマップは常にインラインで生成されます。
* `--production`モードでコンパイルした場合、ミニファイされ、ソースマップは生成されません。