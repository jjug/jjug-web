# JJUG Webページ

JJUG公式サイト (www.java-users.jp) のソースコードを管理するリポジトリです。JJUGスタッフに限らず、どなたでもプルリクを送っていただくことができます。

## 個人環境での動作確認手順

- 事前に必要なもの
    - Hugo: https://gohugo.io/
- 動作確認手順
    1. このリポジトリをcloneするかダウンロードする
    2. cloneしたディレクトリ (jjug-web/) にてサーバ起動コマンドを実行  
`hugo server`
    3. ブラウザで http://localhost:1313 にアクセス

## サイトの更新

### ニュースの追加

- content/post/ にMarkdownファイルを追加する
    - ファイル名に厳密な規定はないので、他のファイルに何となく合わせること

### スタッフ情報の変更

- data/staffs.json を編集する
    - 見れば分かるはず

### レイアウトの修正

- まず themes/beautifulhugo/ の中で、変更したい箇所のレイアウトファイルを探す
    - CSSやJSファイルは static/ にある
    - HTMLのパーツは layouts/partials/ にある
- 変更したいファイルを見つけたら jjug-web/static/ や jjug-web/layouts/ にコピーする
    - 既に同名のファイルがある場合は上書きしないこと
- コピー先のファイルを修正する
