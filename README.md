# practice_rye_uv

## インストール方法

```bash
curl -sSf https://rye-up.com/get | bash
```

インストール中にいくつか質問に答えることになるが、英語読みながらノリでやっとけばOK

## pathを通す

```bash
echo 'source "$HOME/.rye/env"' >> ~/.zprofile
echo 'source "$HOME/.rye/env"' >> ~/.zshrc
```

## プロジェクト開始方法

### プロジェクトに移動して下記コマンドを入力

```bash
rye init
```

### pythonのバージョンを指定する

```
rye pin 3.10
```

### 同期？させる

```
rye sync
```

このコマンドを打つと`.venv`や`.lock`が生成される

### ライブラリの入れ方

```
rye add "flask>=2.0"
```

`remove`で消せる

### 導入したライブラリ一覧表示

```
rye list
```

### 実行方法

```bash
rye run python ...
```
