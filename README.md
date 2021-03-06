# PythonによるAIプログラミング入門

---

![表紙](artificial-intelligence-with-python-ja.png)

---

本リポジトリはオライリー・ジャパン発行書籍『[PythonによるAIプログラミング入門](http://www.oreilly.co.jp/books/9784873118727/)』（原書名『[Artificial Intelligence with Python](https://www.packtpub.com/big-data-and-business-intelligence/artificial-intelligence-python)』）のサポートサイトです。


## サンプルコード

### ファイル構成

|フォルダ名   |説明  |
|:--          |:--   |
|`Chapter 1`  |1章で使用するデータと`.ipynb`形式のノートブック   |
|`...`        |`...`                                             |
|`Chapter 16` |16章で使用するデータと`.ipynb`形式のノートブック  |
|`Appendix A` |付録Aで使用するデータと`.ipynb`形式のノートブック |

サンプルコードの解説は本書籍をご覧ください。

## Pythonと外部ライブラリ

ソースコードを実行するには、下記のソフトウェアが必要です。

* Python 3
* NumPy
* SciPy
* Matplotlib
* Jupyter Notebook

本書では、以下の環境で動作確認しました。

* Windows 10
* Anaconda3（Python 3.6.7）

Anacondaでは、次のパッケージはインストール済みです。

```
numpy
scipy
scikit-learn
matplotlib
jupyter
sympy
nltk
pandas
```

Anacondaでパッケージを追加する場合には、`pip`よりも`conda`を優先して使います。
`conda install`でインストールできるパッケージは次のとおりです。

```
gensim
cvxopt
opencv
tensorflow
```

なお、現時点ではcvxoptとtensorflowは、Pythonの最新バージョン3.7には対応しておらずインストールできません。
その場合には、次のように、Python 3.6の環境を作ります。

```
$ conda create -y -n py36 python=3.6 anaconda cvxopt tensorflow
$ activate py36
```

`pip install`でインストールする必要があるパッケージは次のとおりです。

```
pandas_datareader
kanren
simpleai
deap
easyai
hmmlearn
pystruct
neurolab
gym
```

AIは進歩が激しいため、頻繁にパッケージがバージョンアップされます。
そのため本書のサンプルコードを実行すると、警告やエラーが表示されることがあります。
そのような場合には、まずパッケージのバージョンを最新化してください。
パッケージのバージョンアップは、次のコマンドで行います。

```
// pipの場合：
$ pip install -U パッケージ名

// Anacondaの場合：
$ conda update パッケージ名
```

APIがdeprecated（廃止予定）であるという警告が表示された場合には、
警告メッセージを読んで新しいAPIに書き換えなければならないこともあります。


## 実行方法

学習モデルを構築するためには、代表的な実データが必要です。
必要なパッケージがインストール済んでいれば、パッケージを通じてデータを扱うことができます。

端末に次のように入力して、`jupyter notebook`を起動してください。

```bash
$ jupyter notebook
```

すると、Webブラウザが起動してjupyterのページが開き、
jupyterを起動したフォルダのファイル一覧が表示されます。

サンプルコードを開き、
画面上部の［Cell］メニューから選択するか画面上部のボタンを押して実行します。

右上のメニューから［New▼］→［Python 3］を選択すると、
「Untitled」タブが新たに開きます。
`In [ ]:`の右側にPythonのコードを記述し、
画面上部の［Cell］メニューから選択するか画面上部のボタンを押して実行することもできます。


## 正誤表

まだありません。誤植など間違いを見つけた方は、japan@oreilly.co.jpまでお知らせください。
