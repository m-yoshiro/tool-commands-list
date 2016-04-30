# tool-commands-tips
よく使うツールのよく使うコマンドをリストアップ

- [node.js](#nodejs)
- [Ruby](#ruby)
- [Homebrew](#homebrew)
- [Git](#git)

## node.js

### npm
ツール管理
- npm i -y
- npm i -D [module-name]
- npm i -S [module-name]
- npm update -g npm

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
