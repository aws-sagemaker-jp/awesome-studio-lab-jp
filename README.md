# SageMaker Studio Lab Community

<p align="center">
  <img src="./images/what_is_studio_lab.png" width="300px">
</p>

**[Amazon SageMaker Studio Lab](https://aws.amazon.com/jp/builders-flash/202205/awsgeek-sagemaker-studio-lab/)は、無料かつ簡単にデータサイエンスを学び始めることができる環境です。**

🆓 **Free**
* Amazon SageMaker Studio Labは無料で利用ができます。必要なのはメールアドレスのみです。

:octocat: **Open**
* Studio Labはオープンソースの[JupyterLab](https://jupyterlab.readthedocs.io/en/stable/)をベースにしています。
* コードの補完や見出しの作成など、コミュニティで開発された便利な拡張機能も利用できます。

🔰 **Easy**
* Pythonが実行できる、Jupyter Notebookが作成できる環境があらかじめ構築されています。
* Gitが標準でインストールされており、GUIからも使用できます。

📚 **Community**
* コミュニティを通じて、Studio Labでデータサイエンスが学べる教材やデータ分析の実装が共有されています。
* [GitHub](https://github.com/topics/amazon-sagemaker-lab)で検索して見つけることもできます。


🚀 **SageMakerへの移行が可能**
* Studio Labで作成したプロジェクトは、AWSのSageMakerへ移行することができます。
* **学ぶだけでなく活用したい**方にとって必要なサービス機能と学習教材を提供しています。

<p align="center">
  <h3><a href="./README_usage.md">"Amazon SageMaker Studio Lab の使い方"から利用を開始できます。</a></h3>
</p>

## Studio Labで学べる教材

本リポジトリでは、[データサイエンティスト協会の定義](https://www.datascientist.or.jp/dskentei/)を参照し**データサイエンス**、**データエンジニアリング**、**ビジネス**の3つのカテゴリに分けて教材を紹介します。

Studio LabでJupyterLabで動かせる教材はStudio Labで動かせますが、特に「Open in Studio Lab」のボタンがあると簡単にStudio Labで開くことができます。Open in Studio Labボタンの設置方法は["Open in Studio Lab ボタンの設置方法"](./README_button.md)をご参照ください。

### データサイエンス

#### [Python早見帳](https://chokkan.github.io/python/index.html)

東京工業大学 情報理工学院で使用されている機械学習の教材です。Pythonの基本的な文法はもちろん、Numpy、Matplotlibといった機械学習に欠かせないライブラリの使い方についても解説されています。

教材の詳細とStudio Labでの学び方は、[Python 早見帳が SageMaker Studio Lab からすぐに学べるようになりました](https://aws.amazon.com/jp/blogs/news/python-hayamicho-is-available-in-sagemaker-studio-lab/)をぜひ参照してください。

#### [機械学習帳](https://chokkan.github.io/mlnote/index.html)

Python早見帳と同じく、東京工業大学 情報理工学院で使用されている機械学習の教材です。教材内容の解説と確認問題の実装を[mlnote-note](https://github.com/icoxfog417/mlnote-note)で公開しています。

教材の詳細とStudio Labでの学び方は、[機械学習帳が SageMaker Studio Lab からすぐに学べるようになりました](https://aws.amazon.com/jp/blogs/news/mlnote-sagemaker-studio-lab/)をぜひ参照してください。

#### [ゼロからはじめるデータサイエンス入門（講談社）](https://github.com/taroyabuki/fromzero)

プログラミングの基本、統計入門、前処理、機械学習などを、R・Python対訳・対照で学ぶ書籍です。書籍に掲載されたコードのほかに、[Amazon SageMaker Studio Labのための仮想環境構築法](https://github.com/taroyabuki/fromzero/tree/main/addendum/sagemaker)もサポートサイトで公開されています。GPUを使った深層学習もAmazon SageMaker Studio Labで動作確認済みです。

#### [Machine Learning University](https://aws.amazon.com/jp/machine-learning/mlu/)

Amazonが社内の機械学習教育で使用している教材です。自然言語処理、テーブルデータ、画像、決定木の4コースで、それぞれApplied Scientistらによる解説動画、スライド、Notebookが提供されてます。

* [自然言語処理](https://github.com/aws-samples/aws-machine-learning-university-accelerated-nlp)
* [テーブルデータ](https://github.com/aws-samples/aws-machine-learning-university-accelerated-tab)
* [画像](https://github.com/aws-samples/aws-machine-learning-university-accelerated-cv) 
* [決定木](https://github.com/aws-samples/aws-machine-learning-university-dte)

#### [PRML](https://github.com/ctgk/PRML)

[パターン認識と機械学習](https://www.amazon.co.jp/%E3%83%91%E3%82%BF%E3%83%BC%E3%83%B3%E8%AA%8D%E8%AD%98%E3%81%A8%E6%A9%9F%E6%A2%B0%E5%AD%A6%E7%BF%92-%E4%B8%8A-C-M-%E3%83%93%E3%82%B7%E3%83%A7%E3%83%83%E3%83%97/dp/4621061224)の書籍で登場するアルゴリズムの実装を行っているリポジトリです。かなり難しい書籍なので、[awesome-prml-ja](https://github.com/tsg-ut/awesome-prml-ja)で紹介されている各大学の輪講資料も活用して学ぶことをお勧めします。

#### 他教材

* 自然言語処理
   * [BERTによる自然言語処理入門: Transformersを使った実践プログラミング](https://github.com/stockmarkteam/bert-book)
   * [Natural Language Processing with Transformers](https://github.com/manuelyhvh/nlp-with-transformers)
   * [Hugging Face Quick tour](https://huggingface.co/docs/transformers/quicktour)
* 強化学習
   * [ゼロから作るDeep Learning ❹ 強化学習編](https://github.com/oreilly-japan/deep-learning-from-scratch-4)

### データエンジニアリング

#### [データサイエンス100本ノック](https://github.com/The-Japan-DataScientist-Society/100knocks-preprocess)

小売のPOSデータを題材に、SQLを使用したデータの抽出方法を学べる教材です。SQL以外にも、Pythonの表計算ライブラリであるpandasやRによる実装方法も解説されています。[データサイエンス100本ノック構造化データ加工編ガイドブック](https://www.amazon.co.jp/dp/4802613563)として解説の書籍も発売されています。

教材の詳細とStudio Labでの学び方は、[データサイエンス100本ノックがStudio Labからすぐに学べるようになりました](https://aws.amazon.com/jp/blogs/news/100knocks-preprocess-sagemaker-studio-lab/)をぜひ参照してください。

#### [入門 機械学習パイプライン](https://github.com/oreilly-japan/building-ml-pipelines-ja)

本番環境で機械学習モデルを運用するために、学習データの取り込みからモデルのデプロイまで一連のプロセスを自動化するパイプラインを構築する方法を解説した書籍です(モデルの構築よりはデータに絡むため、こちらのセクションで紹介しています)。TensorFlow Extendedを使用してパイプラインを実装する方法、またクラウド環境にデプロイする方法が学べます。付録ではUberやSpotify、Netflixなど著名な企業のパイプラインの構築事例を参照することができます。

教材の詳細とStudio Labでの学び方は、[「入門機械学習パイプライン」にSagemaker Studio Labで入門する](https://aws.amazon.com/jp/blogs/news/intro-to-mlops-sagemaker-studio-lab/)をぜひ参照してください。

#### データサイエンティストのための Git 入門 [Part1](https://aws.amazon.com/jp/builders-flash/202207/git-introduction-for-data-schientist/?awsf.filter-name=*all) / [Part2](https://aws.amazon.com/jp/builders-flash/202209/git-introduction-for-data-schientist-2/?awsf.filter-name=*all)

開発したモデルをサービスへ組み込むときアプリケーション開発チームと協力することになりますが、協力するうえで知っておくべきチーム開発のためのGitの機能を重点的に紹介した記事です。Part1ではGitの基本的な使い方、Part2ではPull Requestの送り方などを中心に解説しています。[いちばんやさしいGit&GitHubの教本](https://www.amazon.co.jp/%E3%81%84%E3%81%A1%E3%81%B0%E3%82%93%E3%82%84%E3%81%95%E3%81%97%E3%81%84Git-GitHub%E3%81%AE%E6%95%99%E6%9C%AC-%E4%BA%BA%E6%B0%97%E8%AC%9B%E5%B8%AB%E3%81%8C%E6%95%99%E3%81%88%E3%82%8B%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B3%E7%AE%A1%E7%90%86-%E5%85%B1%E6%9C%89%E5%85%A5%E9%96%80-%E3%80%8C%E3%81%84%E3%81%A1%E3%81%B0%E3%82%93%E3%82%84%E3%81%95%E3%81%97%E3%81%84%E6%95%99%E6%9C%AC%E3%80%8D%E3%82%B7%E3%83%AA%E3%83%BC%E3%82%BA/dp/4295013617)著者による、アニメーション画像を使ったわかりやすい記事になっています。

* Part1: [データサイエンティストのための Git 入門](https://aws.amazon.com/jp/builders-flash/202207/git-introduction-for-data-schientist/?awsf.filter-name=*all)
* Part2: [データサイエンティストのための Git 入門 チーム開発編](https://aws.amazon.com/jp/builders-flash/202209/git-introduction-for-data-schientist-2/?awsf.filter-name=*all)

### ビジネス

#### [ML Enablement Workshop](https://github.com/aws-samples/aws-ml-enablement-workshop)

プロダクトを開発するチームが、課題解決の選択肢として機械学習を選択できるようになることをゴールとしたワークショップです。プロダクトマネージャー向けの機械学習入門、ソフトウェア開発者向けハンズオン、プロダクトマネージャー/ソフトウェア開発者/データサイエンティストを交えて行う機械学習のユースケース発見アイデアソンの3つから構成されます。資料はすべてGitHubで公開されています。

#### 金融業界での活用

##### [ESG評価に対する自然言語処理の活用Workshop](https://github.com/aws-samples/aws-esg-evaluation-handson)

企業の開示情報から、ESG評価に関わる記載を抽出するのに自然言語処理を活用する方法を学べるワークショップです。ESG評価の動向と、実際手を動かすハンズオンの2つから構成されています。MSCIやFTSE、RobecoSAMなど代表的な評価機関で採用されているチェックリストを持ちたESG評価手法をベースにしています。

##### [決算短信セグメント情報のデータ抽出ハンズオン](https://github.com/JapanExchangeGroup/FinancialResultsHTML-DataExtraction)

HTML化された決算短信からセグメント情報を抽出する方法が学べるハンズオンです。HTML化された決算短信は、[適時開示情報閲覧サービス](https://www.release.tdnet.info/inbs/I_main_00.html)や、[東証上場会社情報サービス](https://www.jpx.co.jp/listing/co-search/index.html)で公開されています。BeautifulSoupを用いたHTMLからの情報抽出を基礎から学ぶことができます。

## Studio LabからSageMakerへの移行

大規模なデータの前処理や学習が必要になっときは、Studio LabからSageMakerへ移行することができます。

![studio_lab_to_sagemaker.png](./images/studio_lab_to_sagemaker.png)

* [Export Amazon SageMaker Studio Lab environment to Amazon SageMaker Studio](https://docs.amazonaws.cn/en_us/sagemaker/latest/dg/studio-lab-use-migrate.html)
   * ※日本語版作成中

## 採用事例

Studio Labを採用頂いている授業や事例を紹介します。

* [Juliaで学ぶ最適化と機械学習（2024）](https://matsui528.github.io/julia_opt_ml_2024/)
* [4840-1054: Media Computing in Practice (Summer 2022)](https://media-comp.github.io/2022/)
* [NLP若手の会 (YANS) 第17回シンポジウム ハッカソン](https://yans.anlp.jp/entry/yans2022hackathon)
* [岐阜大学　2022実践データサイエンティスト育成事業](https://sites.google.com/db.info.gifu-u.ac.jp/ds2022/%E3%83%9B%E3%83%BC%E3%83%A0/aws%E8%AC%9B%E7%BF%92%E4%BC%9A%E9%AB%98%E5%BA%A6%E3%83%97%E3%83%AD%E3%82%B0%E3%83%A9%E3%83%9F%E3%83%B3%E3%82%B0?authuser=0)

## 関連記事検索

* [Qiita](https://qiita.com/tags/sagemakerstudiolab)
* [Zenn](https://zenn.dev/topics/sagemaker)
* [Twitter](https://twitter.com/search?q=lang%3Aja%20SageMaker%20Studio%20Lab&src=typed_query&f=live)

## リンク

* [aws/studio-lab-examples](https://github.com/aws/studio-lab-examples)

## Disclaimer

本リポジトリのメンテナンスを行っているメンバーはAWSに所属していますが、コミュニティ活動の一環として行っておりAWSの事業とかかわりはありません。

教材の追加やリポジトリ内のコンテンツの修正は[Issues](https://github.com/aws-studiolab-jp/awesome-studio-lab-jp/issues)、また[Pull Requests](https://github.com/aws-studiolab-jp/awesome-studio-lab-jp/pulls)よりお送りください。
