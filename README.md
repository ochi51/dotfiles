# M1 Mac 初期環境構築用(2022/02)

## Mac の設定変更

- ソフトウェアアップデートがないか確認
- システム環境設定を変更
  - `共有` でコンピュータ名を変更
  - `Dockとメニューバー` を好みの設定に変更
  - `キーボード` `トラックパッド` を好みの設定に変更
  - `セキュリティとプライバシー - 一般` で `スリープとスクリーンセーバの解除にパスワードを要求` を `開始後すぐに` に変更
  - `Mission Control` の設定を下記を参考に変更

<img width="664" alt="Mission Control" src="https://user-images.githubusercontent.com/5582393/152388661-fbaee362-c5a2-4925-a405-43f59c0aa1a0.png">


## Xcode のインストール

`Xcode` そのものというより、一緒にインストールされる `Command Line Tool for Xcode` が Homebrew など様々なパッケージで必要

- App Store にログイン
- App Store で `xcode` を検索しインストール


## Display Menu

- Display Menu を App Store で検索し、インストール
- Display Menu を起動し、画面サイズを好みのサイズに変更


## Homebrew

- [Homebrew](https://brew.sh/index_ja) のインストール手順に従いインストール.
- ログに表示される PATH 指定のコマンドを実行

```.bash
brew -v
```

を実行し、実行できればインストール完了

## パッケージのインストール

[Brewfile](/blob/master/Brewfile) の定義されているパッケージをインストール.

- `~` で `Brewfile` を作成して `Brewfile` の内容をコピペするか、 `git clone` して使う.

```.bash
brew bundle
```

- パスワードを求められるので都度入力

ここで `iterm2` にターミナルを変える.


## Google 日本語入力

- `システム環境設定 - キーボード - 入力ソース` で、`+` より `ひらがな(Google)` を追加

<img width="666" alt="キーボード-入力ソース" src="https://user-images.githubusercontent.com/5582393/152386768-619dfa4a-0e8d-4484-8137-c1d3b6fa2ad5.png">


## iterm2

@todo

## Zsh

シェルは Zsh を使う.
brew で `zsh` `zsh-lovers` `zsh-completions` `powerlevel10k` はインストール済み

### Oh My Zsh

[Oh My Zsh](https://ohmyz.sh/#install) のインストール手順に従いインストール.

### Zinit

[Zinit](https://github.com/zdharma-continuum/zinit#automatic-installation-recommended) のインストール手順に従いインストール.

### .zshrc の変更

- [.zshrc](/blob/master/.zshrc) の内容を `~/.zshrc` にコピペ.
- `iterm2` を再起動


## IDE（エディター）

[JetBrains](https://www.jetbrains.com/) のIDEを利用する.
([学生など無料で利用できる場合もある](https://www.jetbrains.com/ja-jp/store/#discounts))

- `JetBrains Toolbox` が `brew` でインストールされているので、起動し必要なツールをインストール


## Git

### Github ssh

Github を ssh で利用可能に設定する.

- [手順](https://docs.github.com/ja/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) に従い、新しい SSH キーを生成して ssh-agent に追加する
- [手順](https://docs.github.com/ja/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) に従い、GitHub アカウントへの新しい SSH キーの追加

以下を実行し、成功したら設定完了

```.bash
ssh -T git@github.com
```

### gitignore_global

gitignore は Nodejs 環境をよく利用する想定.

- `touch ~/.gitignore_global` でファイル作成
- [.gitignore_global](/blob/master/.gitignore_global) の内容を `~/.gitignore_global` にコピペ.

### gitconfig

- `touch ~/.gitconfig` でファイル作成
- [.gitconfig](/blob/master/.gitconfig) の内容を `~/.gitconfig` にコピペし、user.name, user.email を変更.


## ブラウザー

デフォルトのWebブラウザーは Chrome を使用する.

- `brew` でインストールされているので、起動しデフォルトに指定


## ログイン時自動起動設定

`システム環境設定 - ユーザーとグループ - ログイン項目`

<img width="660" alt="自動起動設定" src="https://user-images.githubusercontent.com/5582393/152389336-1cb633ae-6ed6-464c-b8c5-476f6ca2f94e.png">


## BetterTouchTool

@todo


## Karabiner-Elements

@todo

## プログラミング言語別設定

@todo
