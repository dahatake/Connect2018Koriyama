# Connect 2018 in Koriyama - Microsoft 技術たち

Connect 2018 in Koriyama, with UDC （ハッカソン）で参考になる技術情報です。

課題: 地域課題解決アプリを作ろう」～オープンデータを活用して～



Hackathon 進め方 - 例:

1. ビジネス課題を固める
2. 解決の仮説を立てる
3. 解決をするためのシステム構成 (アーキテクチャー)を固める
4. 担当わけ
5. 実現技術(製品)の学習
    1) クイックスタート | チュートリアル を実施
6. 課題解決と選定技術での実現性を確認


# ビジネス課題とその解決の参考 (特にAIを使ったもの)

  - 日本マイクロソフト : YouTube 公式チャネル : Microsoft AI

   https://www.youtube.com/playlist?list=PL1RqQ3kddIpZTMAXfqSy_UHpjVhPiBfSf

# 開発ツール

使い慣れたツールを使ってください。以下は、あくまで「便利」なツールとしてのご紹介です。

1. Visual Studio Code

    Windows | Mac 双方で動作するコーディングツールです。拡張機能が豊富に提供されているため、多様な開発シナリオに対応できます。

    https://code.visualstudio.com/

2. Azure Notebook

    Jupyter Notebook の無料ホスティング環境です。GPUは残念ながら未対応ですw

    https://notebooks.azure.com/

# 開発環境としての Azure 

無償アカウント があります。

https://azure.microsoft.com/ja-jp/free/


Azure 無償アカウントのよくある質問:

https://azure.microsoft.com/ja-jp/free/free-account-faq/

# Azure の無料トレーニング

オンラインで提供されています。その場で実行できる環境がある教材もあります。

https://docs.microsoft.com/ja-jp/learn/azure/

# 実現システムのアーキテクチャを考える

構想アーキテクチャーを Azure で実現する上での参考となります。

https://azure.microsoft.com/en-us/solutions/architecture/

# AI
機械学習、深層学習といった技術によって、これまで実現が難しかった課題を解決します。画像認識、音声認識、言語認識など。主に出来る事は、数値(値、日付など)の予測、分類・仕分け などがあります。

  - Cognitive Services

    学習済みの Deep Learning のモデルを REST API で使えるようにしています。

    https://docs.microsoft.com/ja-jp/azure/cognitive-services/

  - Bot Framework

    Chat Bot を作るためのコーディングベース の Framework です。Cognitive Services の Speech + Translator | LUIS などと組み合わせると Smart Speaker 用のアプリケーションの開発が出来ます。

    https://dev.botframework.com/

  - Cognitive Services | Bot Framework のチュートリアル (マイクロソフト大森さん)

    https://qiita.com/annie


  - Azure AI Gallery

    リコメンデーションなど、独自の機械学習のモデルを作成する際の参考となる、テンプレートがあります。機械学習自体を理解している方であれば、お役に立つと思います。

    https://gallery.azure.ai/


## Web Application

一般的な Web - DB アプリケーション のホスティング環境です。

  1. Azure Web App
  フルマネージドのWebアプリケーションのホスティング環境 (PaaS) です。

      https://docs.microsoft.com/ja-jp/azure/app-service/

  2. Azure SQL Database
  RDBMS の決定版!

      https://docs.microsoft.com/ja-jp/azure/sql-database/

  3. Cosmos DB
  様々なデータモデル (JSON document, Graphなど) を保存できるデータベースです。

      https://docs.microsoft.com/ja-jp/azure/cosmos-db/

## Serverless

サーバーをあまり意識せずに、以下にフォーカスをしてアプリケーション開発が出来ます。
- コード
- コードの実行タイミング。よく使うのは、ファイルが保存された時。タイマーで5分ごと。など。
- データベース、ファイルなどのデータの入出力

1. Azure Functions
  
    コーディング前提の Serverless 環境です。Azure Web App上で動作しています。

    https://docs.microsoft.com/ja-jp/azure/azure-functions/

  2. Logic App
  
      GUIベースの Serverless 環境です。連携先が豊富です。Azure Web App上で動作しています。

      https://docs.microsoft.com/ja-jp/azure/logic-apps/

# Data 関連

  1. Azure Data Factory

      オンプレミス、クラウド上を含めた、様々なデータのコピージョブ作成ツールです。スケジューラーもあります。

      https://docs.microsoft.com/ja-jp/azure/data-factory/