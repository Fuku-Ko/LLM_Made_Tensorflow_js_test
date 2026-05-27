# LLM_Made_Tensorflow_js_test
Tensorflow.jsをAI生成コードで試してみたもの

# 使い方

## オンライン版

以下のリンクをクリックして試してみてください。

https://fuku-ko.github.io/LLM_Made_Tensorflow_js_test/

## オフライン版（ローカル版：本命）

以下の構成を想定します。

```
my-ml-app/
├── index.html               (下記で生成するコードを貼り付けたファイル)
│
└── js/                      (ライブラリ用フォルダ)
    ├── tf.min.js            (TensorFlow.js)
    ├── chart.umd.js         (Chart.js)
    └── papaparse.min.js     (PapaParse)
```

index.htmlをダウンロード、またはコードをコピーして、PCの分かる場所に保存してください。

保存した場所とおなじところ（ディレクトリ）に js という名前のフォルダを作成してください。

jsの中に、以下の3つのファイルを作成してください。

以下のリンクから右クリックし、「名前を付けて保存」等で、それぞれのファイルを js フォルダの中に保存してください。


   tf.min.js:
   https://cdn.jsdelivr.net/npm/@tensorflow/tfjs@4.10.0/dist/tf.min.js


   chart.umd.js:
   https://cdn.jsdelivr.net/npm/chart.js@4.4.0/dist/chart.umd.js


   papaparse.min.js:
   https://cdn.jsdelivr.net/npm/papaparse@5.4.1/papaparse.min.js


index.htmlを開くと、オフライン版を選択できるようになっているはずです。

# 考え方

## 目的

機械学習やディープラーニングの基礎的な部分を最も手軽に体感できること。

## できること

■　機械学習の一連の流れ（学習・推論・運用）を体感する。

■　単純な予測モデルとしてのニューラルネットワーク（NN）の動作を手軽に体感できる。

■　それなりの精度を実現できる。

## 意図していないこと

◆　EDA（探索的データ解析）をすること。

◆　最高性能を目指すこと。

## アプリケーションとしての作り方

「誰でもすぐ使える」を最重要事項に置いています。

そのため、効率やモデル性能をある程度犠牲にしても良いということが、このアプリ作成の前提になっています。

## 開発言語

JavaScript (HTML+JavaScript+CSS)にて作成されています。

ブラウザで動作するという特長があり、「とりあえず動かしてみる」ことにおいては非常に優れており、

アプリのフロント（表層）開発言語として人気です。

## モデル

ニューラルネットワーク（NN）によっています。ライブラリとしてTensorflow.jsを用いています。

## 学習

一般的なk分割交差検証(アンサンブル学習)を実装しています。


