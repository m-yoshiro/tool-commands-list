# tool-commands-tips
よく使うツールのよく使うコマンドをリストアップ

- [node.js](#nodejs)
- [Ruby](#ruby)
- [Homebrew](#homebrew)
- [Git](#git)

## node.js

### npm
ツール管理
ex) npm init -y

| Commands | Usages |
| -------- | -------- |
| init -y | package.jsonファイルを作成。 |
| install(i) | package.jsonを参照しモジュールのインストールを実行 |
| install --save(S) [module] | 指定したモジュールをインストールし、かつpackage.jsonにdependencyとして保存する |
| install --save-dev(D) [module] | 上とほぼ同じ動作だが、dev-dependencyとして保存される |
| update -g npm | npm自身をアップデート |


### nodebrew
バージョン管理
- nodebrew ls-remote
- nodebrew install-binary v0.x.x
- nodebrew use v0.x.x
- nodebrew migrate-package v0.xx.xx


## Ruby

### rbenv
バージョン管理
- rbenv install -l
- rbenv install 2.x.x
- rbenv global 2.x.x
- rbenv rehash

### bundler
ツール管理
- bundle init
- bundle install

Gemfileを参照しローカルの指定したディレクトリにインストール
- bundle install --path vendor/bundle

bundleでインストールしたローカルモジュールを実行
- bundle exec [module-name]

## Homebrew

### Homebrew
ツール管理
- brew install [name]
- brew tap
- brew tap [name]
- brew update
- brew upgrade
- brew unlink [name]
- brew link [name]
- brew list
- brew doctor

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
