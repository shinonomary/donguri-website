# これは何
これはどんぐりの吹奏楽団のwebサイトを公開しているレポジトリです。

# 環境のインストール方法
以下が必要です。
- Git
- Hugo
- Dart Sass
- Go

Gitのインストールは各自検索してインストールすること。
（Macの場合はHomebrewがおすすめ）

Hugoのインストールも[公式](https://gohugo.io/getting-started/installing/)ページを見るべし。
Windows には Chocolatey、Mac では Homebrew がおすすめ。

Dart Sassは以下のコマンドで
とりあえずMac版だけ
```
$ brew install sass/sass/sass
```

Go
```
brew install go
```
or 
https://go.dev/dl/
からインストール


# 初回手順
1. Hugoのプロジェクトファイルを生成する
```
$ cd donguri-website (Gitのルートへ)
$ hugo new site donguri-web
$ cd donguri-web
```

2. テーマの適用
今回は[Paige](https://themes.gohugo.io/themes/paige/)というテーマを選択する。
基本的に以下のコマンドを叩けばOK

```
$ cd donguri-web
$ hugo mod init github.com/shinonomary/donguri-website
$ hugo mod get github.com/willfaught/paige@latest

```
※ちょっと前のhugoのバージョンだと、gitのgit submoduleで導入するのが一般的だったけど、最近のバージョンだとHugo modulesという機能を使うのが一般的になったらしいので、
そちら側で書く。

# 編集作業

2. 新しいPostを作る
```
$ hugo new yourpost.md
```
※ Content配下に勝手に生成されます。


```
: