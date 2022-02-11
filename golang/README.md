
## goenv

### インストール

HomeBrew の `goenv` だと M1 Mac 対応のバージョンをインストールできないため直接インストールする.

```.bash
git clone https://github.com/syndbg/goenv.git ~/.goenv
```

### PATH

`.zshrc` に以下を追加

```.bash
export GOENV_ROOT="$HOME/.goenv"
export PATH="$GOENV_ROOT/bin:$PATH"
eval "$(goenv init -)"
```

## Go

最新バージョンをインストール

```.bash
goenv install -l
goenv install 1.17.6
goenv global 1.17.6
go version
```

## Hugo 等

```.bash
brew bundle --file Brewfile.golang
```
