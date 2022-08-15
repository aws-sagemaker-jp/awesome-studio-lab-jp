# Amazon SageMaker Studio Lab の使い方

Amazon SageMaker Studio Labを使い始めるステップを解説します。

1. アカウントを作成する
2. ログインする
3. Jupyter Notebookを動かす
4. 教材を開く
5. リポジトリを作成する
6. Studio Labをより便利に使う
   * 日本語化する
   * JupyterLabの拡張を導入する
       * Jupyter Notebookでコード補完を行う
       * Jupyter Notebookでコードフォーマットを行う
7. AWSへ接続する
8. リファレンス 

## アカウントを作成する

はじめにStudio Labのアカウントを作成します。アカウントの申し込みは次のフォームから行えます。

**[アカウント作成フォーム](https://bit.ly/3kIjuZL)**

アカウントを申し込むと`no-reply@studiolab.sagemaker.aws`から次の順でメールが届きます。

1. `Account request confirmed`
   * アカウントの申し込みが受け付けられた連絡です。5営業日以内に結果が通知されます。
2. `Account request approved`
   * 申し込みが承認された連絡です。承認から7日以内にアカウント作成を行ってください。この連絡がなかなか来ない、という場合は[問い合わせフォーム](https://pages.awscloud.com/GLOBAL_PM_PA_amazon-sagemaker_20211116_7014z000000rjq2-registration.html)から連絡してください。
3. `Verify your email`
   * アカウント作成後にメールアドレスの認証を行います。メール内のリンクからメールアドレスを認証してください。
4. `Your account is ready`
   * お待たせしました！利用開始いただけます。

大学の授業などで一括でアカウントを作成したい場合は一括承認用の手立てがあります。詳細は[大規模な講座などでStudio Labのアカウントを発行するにはどうすればよいですか?](https://github.com/aws-sagemaker-jp/awesome-studio-lab-jp/discussions/8)をご参照ください。

## ログインする

Studio Labへのログインは、[Studio Lab のランディングページ](https://studiolab.sagemaker.aws/)から行います。

![signin.PNG](images/usage/signin.PNG)

1. 右上の "Sign in" ボタンを押す。
2. Eメールアドレス/ユーザー名、パスワードを入力する。
3. "Sign in" を押しプロジェクトのページを開きます。

## Jupyter Notebookを動かす

Studio LabではCPU/GPUのいずれかでJupyter Notebookを実行することができます。CPUは12時間/セッション、GPUは4時間/セッションです。GPUは24時間以内8時間までという制約があります。

CPU/GPUインスタンスの起動方法は次の通りです。

1. Studio Lab にサインインしたら、このようなプロジェクトページが表示されます。
   * ![Studio Lab Project](https://docs.aws.amazon.com/sagemaker/latest/dg/images/studio-lab-overview.png)
1. "My Project" 以下の "Select compute type" から `CPU`か`GPU` を選択します。
1. "Start runtime" を押します。
1. ランタイムが開始したら "Open project" をクリックし JupyterLab 環境を開きます。

インスタンスを起動すると、JupyterLab のインターフェイスを拡張したStudio LabのUIが開きます。使い方はJupyterLabと同様で、拡張機能のインストールも可能です。UIになじみのない方は [The JupyterLab Interface](https://jupyterlab.readthedocs.io/en/latest/user/interface.html) のページをご覧ください。

![SageMaker Studio UI](https://docs.aws.amazon.com/sagemaker/latest/dg/images/studio-lab-ui.png)

15 GBのストレージが割り当てられるので、ダウンロードしたデータや実行したコード、保存したファイルなどは、後のサインイン時に引き続き利用することができます。

## 教材を開く

Open in Studio Labのボタンが付いた教材を開く手順は次の通りです。

![open_material.png](./images/open_material.png)

1. Studio Labにログインしておく
2. Open Studio Labボタンを押す
3. Runtimeを起動しCopy to Projectする
4. Clone Entire Repoを押し、Clone先を選択
5. "Confirm you want to build..."が出たら「OK」を押す。
   * ※OKを押し忘れたら、`environment.yml`を右クリックし「Build Conda Environment」を実行
6. Notebookを開いて、右上のメニューから作成したKernelを選択し実行する。
   * Notebookにカーネルが表示されない場合は、ターミナルを起動して次のコマンドを実行してみてください。

```
conda activate 環境名
conda install ipython ipykernel
ipython kernel install --user --name 環境名
```

## リポジトリを作成する

新しくリポジトリを作成する時は、テンプレートを使うことで品質の高いリポジトリを手早く作成できます。[datascience-template](https://github.com/icoxfog417/datascience-template)はそのうちの一つです。

![use-template.PNG](./images/usage/use-template.PNG)

他にも、[Cookiecutter Data Science](https://drivendata.github.io/cookiecutter-data-science/)などプロジェクトのテンプレートを生成してくれるツールがあります。新規にプロジェクトを開始する際は、こうしたベストプラクティスに沿ってリポジトリを作るとよいでしょう。

## Studio Labをより便利に使う

### 日本語化する

[JupyterLabの言語パック](https://anaconda.org/search?q=jupyterlab-language-pack)をインストールすることで、部分的に日本語化することができます。

ターミナルを起動し、次のコマンドを実行してください。

```
conda install -c conda-forge jupyterlab-language-pack-ja-jp
```

Settings > Languageから「日本語」が選択できるようになります。

### JupyterLabの拡張を導入する

JupyterLabの拡張を入れることで開発環境をより便利にカスタマイズできます。拡張を有効にするには、拡張管理のセクションで拡張を"Enable"にしてください。

![enable-extension.PNG](images/usage/enable-extension.PNG)

拡張をインストールした後は、JupyterLabを再起動してください。

JupyterLabを再起動します。

![restart-jupyter](images/usage/restart-jupyter.PNG)

### Jupyter Notebookでコード補完を行う

[jupyterlab-lsp](https://github.com/jupyter-lsp/jupyterlab-lsp)の拡張を導入することで、Notebookでコード補完が行われるようにできます。

ターミナルを起動し、次のコマンドを実行してください。

```
conda install -c conda-forge nodejs jupyterlab-lsp python-lsp-server
```

JupyterLab再起動後、Notebookでコード補完が効くようになっているはずです。

![extension-lsp.PNG](images/usage/extension-lsp.PNG)


### Jupyter Notebookでコードフォーマットを行う

[jupyterlab_code_formatter](https://github.com/ryantam626/jupyterlab_code_formatter)を導入することでJupyterNotebook上のコードを成形することができます。`black`と`isort`を使いフォーマットができます。

```
conda install -c conda-forge jupyterlab_code_formatter black isort
```

保存したときに自動的に成形されるようにするには、Settings > Advanced Settings Editor > Jupyterlab Code Formatterから`Auto format config`にチェックを入れてください。


## AWSへ接続する

Studio Labで用意されているCPUやGPU、ストレージが足りなくなった場合AWSと接続することで移行できます。

* Amazon S3: Amazon S3に接続することで15G以上のストレージが利用可能です。詳細は[Amazon S3 に接続](https://docs.aws.amazon.com/sagemaker/latest/dg/studio-lab-use-external.html#studio-lab-use-external-s3)をご参照ください。
* SageMaker Studio: SageMaker Studioに移行することで、Studio Labと同様の使い勝手でAWS上のGPUインスタンスを利用することができます。詳細は[Amazon SageMaker Studio への移行](https://docs.aws.amazon.com/sagemaker/latest/dg/studio-lab-use-migrate.html) を参照してください。

## リファレンス

* [公式ドキュメント](https://docs.aws.amazon.com/sagemaker/latest/dg/studio-lab.html)
* [FAQ](https://studiolab.sagemaker.aws/faq)
