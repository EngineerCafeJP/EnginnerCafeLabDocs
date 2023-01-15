# ホームページを作ろう！

Updata　： 2023-01-14


HPを公開するとは？

レンタルサーバーやVPSを借りてきて、インターネットにホームページを公開する、というのが一般的でした。

いまではこの機能はGitHubにおまかせすることができます。


ちなみにGitHub公式のマニュアルはこちら
https://docs.github.com/ja/pages/getting-started-with-github-pages/creating-a-github-pages-site



# 用意するもの

- Githubのアカウント
- 使い慣れたエディター


# 手順


## 1.Githubにリポジトリを作ろう

トップページに
`https://github.com/{ユーザ名}`として移動する。

New repositoryから任意のリポジトリを建てる。


<img width="1070" alt="image" src="https://user-images.githubusercontent.com/51439199/212525772-8b81a03f-263c-40dd-9ee9-a3309a8c15ad.png">


ポイントとしてはPublicなリポジトリとして選択すること。有料版であればPriviteでもGitHub Pagesを公開することもできる。

つまり、ソースコードは基本的には世界に公開されることになる。


## 2. エディターを用いてパス、ディレクトリとhtmlファイルを記述する

<img width="1389" alt="image" src="https://user-images.githubusercontent.com/51439199/212525900-102af842-5f57-461c-9185-f3f61db5a736.png">

`html テンプレート` などで検索してもいいが、VSCodeを使って`html5`と入力してテンプレートを作成させたほうが早くて便利

![html](https://user-images.githubusercontent.com/51439199/212528088-e4672b8d-f753-41db-a0fd-24fe99a87420.gif)




## 3. リポジトリ設定　からGithubPagesを有効にする



<img width="1378" alt="image" src="https://user-images.githubusercontent.com/51439199/212526142-de44d0e6-6455-4c38-8074-3a69942c9bed.png">

+ HPとして公開したいリポジトリの`Settings`を開く
+ Pagesタブをクリック
+ HPとして公開したいBranchを選ぶ(概ね`main`でOK。フレームワークを使う場合`gh-pages`が推奨される)



`https://{organization名 | ユーザ名}.github.io/{リポジトリ名}/`
とアドレスバーに入力するとページが表示されます。

例えばこのプロジェクトのリポジトリの`web/gettingStartYourHomePage/`を表示したい場合は、

https://engineercafejp.github.io/EnginnerCafeLabDocs/web/gettingStartYourHomePage/


とすれば、`EnginnerCafeLabDocs`リポジトリの`/web/gettingStartYourHomePage/`においた`index.html`の内容が表示されます。


# さらなる研鑽のための情報

Javascriptの各種ライブラリをインストールして使ってみましょう。

CDNという仕組みを利用してWebページに装飾を加えることができる他、npmなどのパッケージマネージャーを用いて依存関係を明確にしたものをGitHub Pagesで動かすことも出来ます。


最近ではjQueryに加えてReactやVueといったレンダリングエンジンが流行っています。


## ファイルを参照したい場合

ローカルでの検証ではXAMPPやhttp-serverなどを利用すると一層開発がしやすいと思います。

CSVやjsonといったファイルを読み込みたい場合にもサーバーを利用する必要があります。

## ログインやフォームの機能をつけたい場合


データの永続化が必要になったらGitHubPagesは概ね卒業です。
データベースなどのミドルウェアを選定できる環境にステップアップしましょう！！






# お仕事に関わる情報


概ね、インターネットで表示できるサイトをつくる仕事に関しては 「Web開発」　「Web制作」　と呼ばれる分野に別れている。
(両者の職掌が曖昧なこともある)



おすすめ書籍
https://book.mynavi.jp/ec/products/detail/id=132319

https://book.mynavi.jp/ec/products/detail/id=65861

