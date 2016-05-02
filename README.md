# tool-commands-tips
よく使うツールのよく使うコマンドをリストアップ

- [node.js](#nodejs)
- [Ruby](#ruby)
- [Homebrew](#homebrew)
- [Git](#git)

## node.js

### npm
ツール管理  

| Commands | Usages |
| -------- | -------- |
| npm | 基本コマンド(以下省略) |
| init | 初期化してpackage.jsonを作成。 |
| init -y | package.jsonの書き込みを省略して初期化。 |
| install(i) | package.jsonを参照しモジュールのインストールを実行 |
| install --save(S) [module] | 指定したモジュールをインストールし、かつpackage.jsonにdependencyとして保存する |
| install --save-dev(D) [module] | 上とほぼ同じ動作だが、dev-dependencyとして保存される |
| update -g npm | npm自身をアップデート |


### nodebrew
バージョン管理

| Commands | Usages |
| -------- | -------- |
| nodebrew | 基本コマンド |
| ls-remote | インストール可能なnode.jsのバージョンを一覧 |
| install-binary v0.x.x | バージョンを指定してバイナリファイルをインストール |
| install v0.x.x | バージョンを指定してインストール |
| use v0.x.x | globalに使用するnode.jsのバージョンを設定 |
| migrate-package v0.xx.xx | 指定したバージョンでインストールしたnpmモジュール全てを現在のバージョンにインストール


## Ruby

### rbenv
バージョン管理

| Commands | Usages |
| -------- | -------- |
| rbenv | 基本コマンド |
| version | 使用中のバージョンを表示 |
| versions | インストール済みのバージョンを一覧 |
| install -l | インストール可能なバージョン一覧 |
| install 2.x.x | 指定したバージョンをインストール |
| global 2.x.x | 指定したバージョンをglobalで使用 |
| local 2.x.x | 指定したバージョンをlocalで指定し、.ruby-versionを作成する |
| rehash | 現在のバージョンでインストール済みのモジュールを使用できるようにする |

### bundler
ツール管理

| Commands | Usages |
| -------- | -------- |
| bundle | 基本コマンド |
| init | |
| install | |
| install --path vendor/bundle | Gemfileを参照しローカルの指定したディレクトリにインストール |
| update | |
| exec [module-name] | bundleでインストールしたローカルモジュールを実行 |

## Homebrew

### Homebrew
ツール管理

| Commands | Usages |
| -------- | -------- |
| brew | 基本コマンド |
| install [name] | |
| tap | |
| tap [name] | |
| update | |
| upgrade | |
| unlink [name] | |
| link [name] | |
| list | |
| doctor | |

## Git
コミット履歴を閲覧
- git log --oneline

指定したコミットの更新内容を閲覧
- git show [ID]

コミットを削除
- git reset --hard HEAD^ 直前のコミットを削除しファイルにも反映

gitの管理から削除
- git rm
- git rm -r
- git rm --cache
- git branch -m [old name] [new name]
