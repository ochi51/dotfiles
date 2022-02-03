Ruby の初期設定
=============

```.bash
rbenv init
```

Stable なインストール候補の表示

```.bash
rbenv install -l
```

最新 Stable version のインストール

```.bash

rbenv install 3.1.0
```

ローカルのバージョンを変更

```.bash
rbenv local 3.1.0
```

確認

```.bash
rbenv versions
ruby --version
```

PATH が通らない場合は、`.zshrc` に以下があるか確認

```.bash
# Ruby rbenv PATH
if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi
export PATH="$HOME/.rbenv/bin:$PATH"
```
