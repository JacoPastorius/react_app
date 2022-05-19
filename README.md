# Webアプリケーションを作ろう

## JavaScriptの学び方と留意

### JavaScriptの要約

- JavaScriptは「コンパイル言語」と違って実行しやすい「スクリプト言語」
- そのため実行のしやすさで初心者のとっつきやすさと、web関係の人使用しているので、多くのノウハウ記事は見つかる
- JavaScript自体にバージョンという考えがなく、規格（書き方）がある
- そのため規格が混在した書き方があるので初心者は混乱することがあるよ

---

### JavaScriptの規格ついて

- JavaScriptの規格はES（ECMAcript）と呼ばれるよ
- ESにはバージョンがあって、今はES6（2015）が支流だよ
- ES6とそれ以降のESのバージョン（ES5）では書き方がガラリと変わる まったく書き方が違う
- その全く違う書き方が混在してもJavaScriptのプログラミングは動いてしまうなのでES6を意識して書いたり読んでねって話。

---

### 基礎を学ぶにいいサイト

- JavaScript Primer
<https://jsprimer.net/intro/>  
※書き方とかいろいろな説明の正しさは基本ここで間違はない
  - いろいろな人がドキュメントを修正追加しているので、最新のjavascriptの教科書
  - リポジトリ<https://github.com/asciidwango/js-primer>

---

### その他

- ES規格についての参考  
<https://qiita.com/minato-naka/items/73b9d531c871d98a3f22> 

---

## 環境構築

### 1．Node.jsのインストール

- まずはNode.jsを使う。Node.jsはjavascriptを実行するために必要なエンジン
- Node.jsの公式サイト
[https://nodejs.org/ja/](https://nodejs.org/ja/)  

#### インストール手順

- [xx.xx.x LTS（推奨版）] ⇒ をクリックでインストーラーをDL
- DL後、インストーラー起動。  
- すべて「次へ(Next)」を選択しインストール  
- インストールで、`node.js`と`npm`がインストールされる。
- `npm`はjavascriptの外部ライブラリの管理などができるパッケージ管理システムだよ。
  - javascriptの外部ライブラリは↓のサイトで管理され、ダウンロードできる。
  - <https://www.npmjs.com/>

#### インストール後の確認※コマンドプロンプトで確認  

- node.jsのバージョン確認  
  `node --version`または`node -v`を入力  

  ```bash
  C:\Users\PCUSER>node --version
  vxx.xx.x
  ```

- npmのバージョン確認  
  npmはjavascriptのpackageマネージャー  
  `npm --version`または`npm -v`を入力 ※バージョンが表示される

  ```bash
  C:\Users\PCUSER>npm --version
  x.xx.x
  ```

#### 【補足】npmコマンド

- `npm init` - 初期化(package.jsonの生成)  

    ```bash
    npm init

    …省略…

    package name: (react_sample)
    version: (1.0.0)
    description:
    entry point: (index.js)
    test command:
    git repository:
    keywords:
    author:
    license: (ISC)

    …省略…

    Is this OK? (yes)
    ```

- `npm install` - 一括パッケージインストール(package.json)  
- `npm install <package_name>` - パッケージインストール  
- `npm install -dev <package_name>` - パッケージインストール  
- `npm uninstall <package_name>` - アンインストール  

---

### React環境構築

- Reactはwebアプリケーションフレームワークだよ。
- 公式サイト<https://ja.reactjs.org/>

- 作業用ディレクトリを作成  

  ```bash
  mkdir dev_react
  cd dev_react
  ```

- reactのアプリケーションを作成  

  ```bash
  npx create-react-app myapp  
  cd myapp
  ```

- アプリケーションサーバーの開始  

  ```bash
  npm start
  ```
