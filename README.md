# SageMaker Studio Lab Community

<p align="center">
  <img src="./images/what_is_studio_lab.png" width="300px">
</p>

Amazon SageMaker Studio Labは、メールアドレスのみ・無料でJupyterLab環境が使えるサービスです。[Amazon SageMaker Studio Lab の使い方](./README_usage.md)にStudio Labのアカウント登録方法や利用方法をまとめています。

本リポジトリでは、Amazon SageMaker Studio Labを使用しMLの基礎から実践まで学んでいくための教材を紹介しています。教材の追加はPull Requestより受け付けておりますので、ガイドラインをご一読の上、[Issues](https://github.com/aws-studiolab-jp/awesome-studio-lab-jp/issues)/[Pull Requests](https://github.com/aws-studiolab-jp/awesome-studio-lab-jp/pulls)よりお送りください。Open in Studio Labボタンの設置方法は["Open in Studio Lab ボタンの設置方法"](./README_button.md)をご参照ください。

## 機械学習を学ぶ教材

JupyterLabで動かせる教材はStudio Labで動かせますが、特に「Open in Studio Lab」のボタンがあるリポジトリは、ボタンを押すことで簡単にStudio Labで開くことができます。以下では「Open in Studio Lab」ボタンを設置いただいている教材を紹介します。

### Python

#### [Python早見帳](https://chokkan.github.io/python/index.html)

東京工業大学 情報理工学院で使用されている機械学習の教材です。Pythonの基本的な文法はもちろん、Numpy、Matplotlibといった機械学習に欠かせないライブラリの使い方についても解説されています。

### 機械学習

#### [機械学習帳](https://chokkan.github.io/mlnote/index.html)

Python早見帳と同じく、東京工業大学 情報理工学院で使用されている機械学習の教材です。教材内容の解説と確認問題の実装を[mlnote-note](https://github.com/icoxfog417/mlnote-note)で公開しています。

#### [ゼロからはじめるデータサイエンス入門（講談社）](https://github.com/taroyabuki/fromzero)

プログラミングの基本、統計入門、前処理、機械学習などを、R・Python対訳・対照で学ぶ書籍です。書籍に掲載されたコードのほかに、[Amazon SageMaker Studio Labのための仮想環境構築法](https://github.com/taroyabuki/fromzero/tree/main/addendum/sagemaker)もサポートサイトで公開されています。GPUを使った深層学習もAmazon SageMaker Studio Labで動作確認済みです。

#### [Machine Learning University](https://aws.amazon.com/jp/machine-learning/mlu/)

Amazonが社内の機械学習教育で使用している教材。自然言語処理、テーブルデータ、画像、決定木の4コースで、それぞれApplied Scientistらによる解説動画、スライド、Notebookが提供されてます。

* [自然言語処理](https://github.com/aws-samples/aws-machine-learning-university-accelerated-nlp)
* [テーブルデータ](https://github.com/aws-samples/aws-machine-learning-university-accelerated-tab)
* [画像](https://github.com/aws-samples/aws-machine-learning-university-accelerated-cv) 
* [決定木](https://github.com/aws-samples/aws-machine-learning-university-dte)

### 画像処理

* [PRML](https://github.com/ctgk/PRML)
  * パターン認識と機械学習本の実装を行っているリポジトリです。

### 自然言語処理

* [BERTによる自然言語処理入門: Transformersを使った実践プログラミング](https://github.com/stockmarkteam/bert-book)
* [Natural Language Processing with Transformers](https://github.com/manuelyhvh/nlp-with-transformers)
* [Hugging Face Quick tour](https://huggingface.co/docs/transformers/quicktour)

### 強化学習

* [ゼロから作るDeep Learning ❹ 強化学習編](https://github.com/oreilly-japan/deep-learning-from-scratch-4)

### MLOps

* [入門 機械学習パイプライン](https://github.com/oreilly-japan/building-ml-pipelines-ja)

### 開発

* [データサイエンティストのための Git 入門](https://aws.amazon.com/jp/builders-flash/202207/git-introduction-for-data-schientist/?awsf.filter-name=*all)


## 機械学習を活用する教材

機械学習を学ぶ段階から活用する段階になると、機械学習以外の知識も必要になります。アプリケーション開発のプロセスや本番環境で要求される非機能要件を満たすための設計方法などです。

Studio Labは本格的な機械学習アプリケーションを開発するためのSageMakerと統合されており、機械学習の学びから本番環境で稼働させるための開発までシームレスに学ぶことができます。

![studio_lab_to_sagemaker.png](./images/studio_lab_to_sagemaker.png)

本セクションでは活用を検討する段階に入ったときに参照する教材を紹介します。

### 機械学習モデル開発基礎

プロダクト開発メンバーの一員として知っておくべき基礎的な知識を学ぶための教材を紹介します。

* [ML Enablement Handson](https://github.com/aws-samples/aws-ml-enablement-handson)

### 機械学習モデル開発実践

分散学習やMLOpsの構築など、本番稼働に欠かせない機械学習モデルの構築技術を学ぶための教材を紹介します。

* (Coming Soon)

## 採用事例

Studio Labを採用頂いている授業や事例を紹介します。

* [4840-1054: Media Computing in Practice (Summer 2022)](https://media-comp.github.io/2022/)


## 関連記事検索

* [Qiita](https://qiita.com/tags/sagemakerstudiolab)
* [Zenn](https://zenn.dev/topics/sagemaker)
* [Twitter](https://twitter.com/search?q=lang%3Aja%20SageMaker%20Studio%20Lab&src=typed_query&f=live)

## リンク

* [aws/studio-lab-examples](https://github.com/aws/studio-lab-examples)

※本リポジトリのメンテナンスを行っているメンバーはAWSに所属していますが、コミュニティ活動の一環として行っておりAWSの事業とかかわりはありません。
