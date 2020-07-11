# Python project using pip and venv

## 使い方

### 仮想環境の作成

VSCode のターミナルで以下のコマンドを実行し、仮想環境を作成します。
わかりにくいですが、最初の`venv`はコマンド、後の`venv`が環境の名前(ディレクトリの名前)です。環境の名前は変更できますが、リポジトリでは管理しないので、`.gitignore`に追記することを忘れないようにしてください。

```
$ python -m venv venv
```

### 仮想環境の有効化

仮想環境を作成したら、仮想環境を有効化(activate)します。以下のコマンドを実行してください。環境の名前を変更している場合は、それに合わせてパスを変更してください。

```
$ source venv/bin/activate
```

### パッケージのインストール

以下のコマンドで、pip のアップデートと必要なパッケージをインストールします。`pip`のアップデートは実施しなくてもよいです。

```
(venv) $ pip install --upgrade pip
(venv) $ pip install -r requirements.txt
```

以下のパッケージがインストールされます。

- flake8
- hacking
- flake8-docstrings
- mypy
- bandit
- pytest
- pytest-cov
