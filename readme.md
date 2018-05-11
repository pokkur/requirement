# 作業環境について事前に確認しておきたいこと

※**太字**は必須内容

## 前提

- [ ] proxyやアクセス制限などの過剰なセキュリティでない環境が望ましい
- [ ] **プルリクエストなどによるコードレビューのフローがある**
- [ ] バックログやtrelloやslackによるタスク管理がなされている
- [ ] コードやドキュメントはgitとgsuitsなどで管理されている
- [ ] **macbook、ディスプレイ、USキーボード**

## マークアップ

最低条件として、scssやstylusなどのcssプリプロセッサと  
pugなどのテンプレートエンジンを利用していること。  
oocssの概念に基づいたcss/html設計になっていること。  
IEやandroidなどの旧ブラウザをサポートする必要がある場合、  
polyfillなどを多用して差異をなくすような方針でないか

### like

- [ ] mixin, extend, functionを適切に使用している（extend不使用）
- [ ] cssスコープ（module）を実現している
- [ ] **airbnbやtrelloなどのメジャーなコーディング規約を採用している**
- [ ] ブラウザサポートが `> 1% in JP`
- [ ] postcss

### hate

- [ ] cssハックを使用している
- [ ] ベンダー・プレフィックスを直書きしている
- [ ] セレクタのネストが無駄に深い
- [ ] scssファイルにスタイルガイド
- [ ] float、clearfixの使用
- [ ] **shift-jis**

## コーディング

es2015による記述がなされているか、もしくは変換できるコードか。  
具体的には、withやevalや8進数表記の使用があったり関数宣言がされていないなど。  
適切にコメントが挿入されていて、ドキュメントやスタイルガイドがあると良い。

### like

- [ ] リテラル構文
- [ ] Promiseやasync/awaitで非同期処理を実装している
- [ ] lighthouseの指摘に則ってる
- [ ] **eslintを通しており、 prettifyで整形されている**
- [ ] 単体テスト

### hate

- [ ] jqueryやlodashなどに完全依存している
- [ ] インラインscript記述の乱用
- [ ] **coffeescript**
- [ ] react

### Next

実績がほしい内容

- [ ] pwa（service worker）
- [ ] webgl
