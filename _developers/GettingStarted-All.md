---
title: InterSystems 製品で開発を始める
date: 2024-12-02
permalink: /GettingStarted-All.html
layout: post
---

InterSystems IRIS® data platform の利用可能なツールや InterSystems IRIS または IRIS for Health を使用したアプリケーションのセットアップと開発の基本について学習できるパスです。

これから InterSystems 製品を利用される開発者を対象に構成されています。

学習項目詳細は以下の通りです。

[1. <img src="./assets/icons/1-IRIS.png" width="40%"/>](#1-)

[2. <img src="./assets/icons/2-serversideapp-better-dicision.png" width="40%"/>](#2-)

[3. <img src="./assets/icons/3-integration.png" width="40%"/>](#3-)

[4. <img src="./assets/icons/4-custom.png" width="40%"/>](#4-)

[5. <img src="./assets/icons/5-access-multilanguage.png" width="40%"/>](#5-)

[6. <img src="./assets/icons/6-APIManagement.png" width="40%"/>](#6-)

[7. <img src="./assets/icons/7-Analytics.png" width="40%"/>](#7-)

[8. <img src="./assets/icons/8-performance.png" width="40%"/>](#8-)


このパスの他に、以下講師付きクラスルームトレーニングコースの受講を推奨いたします。

- <a href="https://www.intersystems.com/jp/intersystems-sql/" target="_blank">InterSystems SQL</a>
- <a href="https://www.intersystems.com/jp/intersystems-object/" target="_blank">InterSystems Object</a>
    - このコースは**ObjectScriptを学習するコースではありません。**
    - InterSystems製品でオブジェクト指向プログラミングを行う方法、また永続クラス定義の作成、オブジェクト操作方法を学習するためのコースです。
- <a href="https://www.intersystems.com/jp/intersystems-server-system-administration/" target="_blank">InterSystems Server システム管理1</a>
- <a href="https://www.intersystems.com/jp/intersystems-server-system-administration-2/" target="_blank">InterSystems Server システム管理2：セキュリティ管理編</a>


---


## 1. <img src="./assets/icons/1-IRIS.png" width="70%"/>

InterSystems IRIS®データ・プラットフォームは、信頼性の高い統一プラットフォームで重要なアプリケーションを迅速に開発・デプロイすることを可能にします。

- InterSystems IRISとは（日本語字幕入りビデオ）

    {% include youtube.html id="w2OeWx3WNOs" %}

<details>
<summary> ▶日本語字幕 </summary>
<div class="transcript">
InterSystems IRIS は統合データ プラットフォームです。
<br>
大規模かつ拡張可能なデータベース、組み込みの分析機能、統合／相互運用性ツール、そして自動化されたメカニズムによりデプロイを容易にします。
<br>
これらのテクノロジーは、貴社のビジネスに重要なアプリケーションの開発とデプロイをさらに迅速化します。
<br>
中核を成す InterSystems IRIS データベースは、高パフォーマンスで大幅な拡張が可能です。
<br>
きわめて効率的なデータ構造により高速化と柔軟性を実現します。
<br>
また直感的な機能を使用してシステムを垂直／水平の両方向に拡張できます。
<br>
InterSystems IRIS は、どんなに大きな問題であろうと対処します。
<br>
InterSystems IRIS は、マルチモデル機能により高い柔軟性を実現します。
<br>
つまり、いかなるコードセットおよびデータセットにおいてもコードが複数の異なるモデルのデータにアクセスできるのです。
<br>
オブジェクト、リレーショナル、ドキュメントだけでなく、基本データ構造へのネイティブアクセスにも対応しています。
<br>
データやコードを分離する必要はなく、すべてを単一の環境から実行できます。
<br>
このクラス最高のデータベース テクノロジーで提供される分析スイートにより、データから有意義な洞察を抽出できるようになります。
<br>
オープンな分析プラットフォームであるため、お気に入りのツールやテクノロジーを接続して組み合わせることができます。
<br>
InterSystems 独自のリアルタイム分析機能やダッシュボードのほか、サード パーティのテクノロジーも接続して利用できます。
<br>
他のデータベースと異なり、リアルタイム分析のためにトランザクションデータと分析データを別々に維持管理する必要はありません。
<br>
InterSystems IRIS はすべてを一括して実行し、モデルをリアルタイムで適用します。
<br>
ほとんどのデータベースは構造化データなら難なく処理できますが、今日では非構造化データが増加の一途をたどっています。
<br>
すなわち、必ずしも厳密に定義されていないデータ、例えば、各種の記事、ソーシャル メディアフィード、医師が書くカルテ、メールなどです。
<br>
このような非構造化データを扱う場合、InterSystems IRIS の自然言語処理機能を使用すれば、ボトムアップのアプローチが可能になります。
<br>
つまり、辞書やオントロジーをあらかじめ定義する必要がなくなります。
<br>
非構造化データ内のコンセプトやリレーションシップを直接そのまま検出できるようになります。
<br>
提供されている API により、主要なコンセプトの特定、ドキュメントの要約、感情の判別、関連トピックの検出などが可能になります。
<br>
InterSystems IRIS は統合データベース プラットフォームであり、オープンなデータベースプラットフォームでもあります。
<br>
パワフルで柔軟な統合エンジンが搭載されているため、人、プロセス、アプリケーション、システムを結び付けられます。
<br>
例えば、3 つの異なるアプリケーションを異なるユーザー集団が使用しているとします。
<br>
見込み客のデータを管理する営業アプリケーション、従業員と顧客の研修を管理する研修アプリケーション、そして顧客のサポート チケットやユーザー プロファイルを管理するサポートアプリケーションです。
<br>
これらのアプリケーションのユーザーとデータは共通していますが、それぞれ異なるアプリケーションです。
<br>
しかし InterSystems IRISなら、これらを完全に相互運用可能です互いに、シームレスにデータを共有してコミュニケーションを図れます。
<br>
さまざまな開発言語のAPI に対応しているため、既存のアプリケーションをInterSystems IRIS に接続して、これらのアプリケーションとの
データの送受信などを行えます。
<br>
既存アプリでどのような言語を使用していても対応できます。
<br>
メッセージ ルーティングにも対応しているため、新しい従業員を採用したときに、メッセージを学習アプリケーションに送信して、その名前と役職の情報を追加できます。
<br>
またデータを変換する場合も、必要な形式のデータを確実に入手できます。
<br>
例えば、あるシステムでは名前が「名姓」の形式で保存されていて、別のシステムでは「姓,名」の形式が使用されている場合、このデータを簡単かつ直感的に、そして適切に変換することができます。
<br>
どのような場合でも、InterSystems IRIS は、変化し続ける各部をシームレスに統合します
<br>
さらに、InterSystems IRIS上で構築されたアプリケーションをデプロイする場合のプロセスも、かつてないほど簡単です。
<br>
自動化されたツールが、パブリックまたはプライベートクラウド、ローカル サーバー、ベアメタル サーバー、または仮想マシンへのインフラのデプロイプロセスを最適化します。
<br>
ビジネスを前進させるアプリケーションを構築するのであれば、InterSystems IRIS 上での構築をお勧めします
</div>
</details>
> ※ NLPについての説明が含まれますが、この機能はバージョン2023.3以降の製品には含まれなくなりました。現在は<a href="https://github.com/intersystems/iknow/" target="_blank">オープンソース版</a>を公開しています。 
{: .block-warning}
<br>

> **IRIS概要についてもう少し詳しく確認されたい方は約30分の以下ビデオをご参照ください。**
>- InterSystems IRIS データプラットフォームのご紹介    
{: .block-warning}
{% include youtube-list.html id="vo12UnH-c-s" list="PLzSN_5VbNaxD-r8wU4LHwLwGSzUjrffEX" %}

<br>
- InterSystems へようこそ

    {% include youtube.html id="v4uoejre5IU" %}

<details>
<summary> ▶日本語字幕 </summary>
<div class="transcript">
InterSystems は、世界で最も重要なアプリケーションを支えるエンジンです。<br>
私たちのお客様は、医療、ビジネス、政府のシステムを円滑に運営しています。世界中の 5 億人以上の人々が、必要な情報への確実なアクセスを提供する当社のテクノロジーに信頼を寄せています。<br>

私たちが構築するすべての製品は、相互運用性（Interoperability）、信頼性（Reliability）、直感性（Intuitiveness）、拡張性（Scalability）という原則を実現しています。私たちのコードはエレガントでシンプルに設計されておりソリューションは効率的です。<br>

私たちは、お客様の成功のために必要なことは何でもします。私たちの最高の人材がお客様からのお問い合わせに対しサポートいたします。<br>

パートナーシップこそが私たちのビジネスの理由です。私たちは個人経営であるため、私たちが行うことはすべてお客様のためでありお客様だけのものです。<br>
クライアントのアプリケーションは、失敗が許されないほど重要なものだからです。<br>
必要なときに必要な情報を確実に入手できるよう、私たちはここにいます。<br>
私たちは、世界を前進させるソリューションを構築します。重要なデータを管理するなら InterSystems にお任せください。
</div>
</details>

---
## 2. <img src="./assets/icons/2-serversideapp-better-dicision.png" width="70%"/>

InterSystems 製品の組み込み言語である InterSystems ObjectScript を使用して、新しいクラスの作成、オブジェクトの操作、SQL クエリの実行について学習します。

このパスを終了すると、ObjectScript を使用してInterSystems製品のサーバーサイド・アプリケーションを構築することができるようになり、以下の開発に役立てることができます。

- データ操作以外の処理も含めたストアドプロシージャの開発
- Interoprabilityで使用するカスタム・ビジネス・コンポーネントの開発
- ビジネスルールとメッセージルータのコードで作成するカスタム関数
- カスタムコードによる高度なデータ変換の作成

カスタム・ビジネス・コンポーネントの構築方法の詳細については[「カスタムコンポーネントを使用したシステム統合の開発」](#4-)をご参照ください。

### はじめに

最初に概要をビデオでご覧ください。

InterSystems IRIS® データプラットフォームのアーキテクチャとクラスの基本を学び、ObjectScript でのコーディングを開始します。

- InterSystems 製品のアーキテクチャ概要 ～ネームスペースとデータベース～

    {% include youtube-list.html id="TNjUnuw8K_Q" list="PLzSN_5VbNaxCWpesN3ulh_EZ9sGkw09q5" %} 

<details>
<summary> ▶日本語字幕 </summary>
<div class="transcript">
こんにちは、InterSystems のテクニカルトレーナーのシェーンです。このビデオでは InterSystems 製品のアーキテクチャについてお話します。<br>
InterSystems 製品のアーキテクチャーについて説明する際、私たちは常に 2 つの主要な概念であるデータベースとネームスペースについて説明しています。<br>

データベースは物理的なファイルです。これらファイルはファイルシステム上のどこかに置かれています。<br>
InterSystems 製品の場合、データベース・ファイルにはデータだけでなくコードも含まれます。つまり、データベースは、データとコードを含むファイルシステム上の物理ファイルで、どこかのディレクトリに存在しています。<br><br>

ネームスペースは、データベース・レイヤの上にある抽象化された論理レイヤで、1 つ以上のデータベース・ファイルを参照します。<br>
新しいネームスペースを作成しようとすると、データ用のデフォルト・データベースとコード用のデフォルト・データベースの設定を求められます。<br>
確認のため、振り返りましょう。<br>
データベースは、データとコードを含むファイル・システム内の物理ファイルです。ネームスペースは、いくつかのデータベースを参照できる抽象化された論理定義です。<br><br>

ユーザがシステムに接続するとき、またアプリケーションが例えば ODBC や JDBC 経由でシステムに接続したり REST サービスや管理ポータルのような Web 接続を行ったり、ターミナルセッションで接続したりします。<br>
ユーザやアプリケーションがシステムへ接続する際、ネームスペースを指定します。<br>

例えば、請求処理を行うアプリケーションがあるとします。<br>
あなたは BILLING ネームスペースから、BILL データ・データベースと BILL コード・データベースに接続しようとします。<br>
この他に、ネームスペースから他のデータベースファイルをマッピングして利用することもできます。<br>
例えば、会計情報を取り扱う FINANCE ネームスペースを見てみましょう。<br>
このネームスペースではデフォルトのデータベースに加え、追加データを操作できるようにマッピングを追加することができます。<br>
また、他のユーザが他のアプリケーションに接続するために使用する他のデータベースを参照する VENDOR という名前のネームスペースも作成できます。<br>
このネームスペースはデフォルトデータベースとして、VEN データ・データベースと VEN コード・データベースを使用しています。<br>

このネームスペースは FINANCE データベースに Mapping されています。<br>
この定義により、ネームスペースに接続しているアプリケーションが FINANCE にあるデータを参照できることを示しています。<br>
そして、アプリケーションが接続している BILLING ネームスペースも同様に、FINANCE データベースのデータを参照できます。<br>
<br>
これは、ユーザとアプリケーションが1つのエントリーポイントでシステムに接続でき、ファイルシステム内のどこにファイルが存在するかという実装の詳細を気にすることなく多くのデータベースファイルからなるコードやデータを利用できるようにしています。<br>
<br>
これが、InterSystems 製品のアーキテクチャです。<br>
より詳細を確認されたい場合は、その他のビデオや記事をご参照ください。
</div>
</details>

### 日本語：セルフラーニングビデオ

オリエンテーションに最適なセルフラーニングビデオやコンテンツをご用意しています。

- 以下動画から、IRIS の開発環境の作成方法、ネームスペース／データベースについて、IDE から IRIS に接続する方法を確認できます。

    ✅ <a href="https://jp.community.intersystems.com/node/478601" target="_blank">【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その2：InterSystems IRIS で開発をはじめよう！</a>

    {% include youtube-list.html id="ID6ImJTgJRk" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %} 
    
<br>
- ObjectScriptの基本操作の学習については、**<a href="https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/Basic.md" target="_blank">[ObjectScript クックブック：ObjectScriptの基本のき！</a>** をご参照ください。
<br><br>
- 以下動画から、クラス定義の作成からインスタンス生成、保存までの流れを確認できます。

    ✅ <a href="https://jp.community.intersystems.com/node/478606" target="_blank">【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その3：IRIS でクラス定義を作ろう（オブジェクト操作の練習）</a>

    {% include youtube.html id="kWJCzn9bndQ" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %} 

<br>
- 以下動画から InterSystems 製品での JSON 操作方法をご確認いただけます。

    ✅ コピー＆ペースト元がある記事：<a href="https://jp.community.intersystems.com/node/480106" target="_blank">【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：IRIS での JSON の操作</a>

    {% include youtube-list.html id="045HRug72VE" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %} 

<br>
- メソッド内で SQL を記述する方法については、以下クックブックをご参照ください。

    ✅ <a href="https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/Basic.md#7-%E3%83%A1%E3%82%BD%E3%83%83%E3%83%89%E3%82%84%E3%83%AB%E3%83%BC%E3%83%81%E3%83%B3%E3%81%A7sql%E3%82%92%E5%AE%9F%E8%A1%8C%E3%81%99%E3%82%8B%E6%96%B9%E6%B3%95" target="_blank">ObjectScriptクックブック：7.メソッドやルーチンでSQLを実行する方法</a>


関連するトレーニングコースは以下の通りです。
- <a href="https://www.intersystems.com/jp/intersystems-object/" target="_blank">InterSystems Object（2日間）</a>
- <a href="https://www.intersystems.com/jp/intersystems-sql/" target="_blank">InterSystems SQL（2日間）</a>
  

> **英語のみとなりますが、以下のオンラインコースもあります。**
>
> - <a href="https://learning.intersystems.com/course/view.php?name=IRIS%20Class" target="_blank">オンラインコース（英語）：Creating an InterSystems Class Definition in VS Code</a>
>
> - <a href="https://learning.intersystems.com/course/view.php?name=Cach%C3%A9%20ObjectScript%20Basics" target="_blank">オンラインコース（英語）:InterSystems ObjectScript Basics</a>
>
> - <a href="https://learning.intersystems.com/enrol/index.php?id=2523" target="_blank">オンラインコース（英語）:InterSystems IRIS Objects Introduction
>
> - <a href="https://learning.intersystems.com/course/view.php?name=Cach%C3%A9%20SQL%20Overview" target="_blank">オンラインコース（英語）：InterSystems SQL Overview</a>
>
> - <a href="https://learning.intersystems.com/course/view.php?name=JSON%20in%20IRIS" target="_blank">オンラインコース（英語）:Using JSON in InterSystems IRIS</a>
>
> - <a href="https://learning.intersystems.com/course/view.php?name=Server-Side%20Application%20Exercise" target="_blank">演習環境付き演習（オンラインコース）：Learning Path Exercise: Building a Server-Side Application with InterSystems IRIS</a>
>
>    InterSystems IRIS® データプラットフォームと InterSystems ObjectScript を使用して小規模なデータベースアプリケーションを作成します。
>    
>    この演習では、InterSystems IRIS を使用したサーバサイド・アプリケーションの構築の学習パスで学習したすべてのスキルを結集して、大規模な書籍コレクションに関する情報を格納および取得するためのクラスを作成し SQL を使用します。
>    
>    この演習は、既存の知識をテストするために学習パスを開始する前にまたはキャップストーン・プロジェクトとして最後にお試しください。
{: .block-tip}


### 認定テスト受験の準備が整ったら・・・

InterSystems Learning Services では、業界標準の認定試験を提供しあなたが InterSystems の技術を習得していることを証明します。

当社の試験は、安全なオンライン試験監督とセルフサービス予約で提供されます。受験者は、いつでもどこでも都合のよいときに試験を受けることができます。

※英語のみ：<a href="https://www.intersystems.com/education/" target="_blank">Exam: InterSystems IRIS Core Solutions Developer Specialist</a>


---
## 3. <img src="./assets/icons/3-integration.png" width="70%"/>

InterSystems 製品の Interoperability(相互運用性)フレームワークにより、インターフェイスエンジニアやソフトウェア開発者は、複数のシステムを接続し下流のアプリケーションにメッセージを迅速にルーティングすることができます。

このパスでは、インテグレーションの基本を学び組み込みオプションとカスタムオプションを使用してデータを送信、受信、処理、変換する方法を確認します。

- <a href="https://learning.intersystems.com/course/view.php?name=Interop%20QS" target="_blank">体験環境付き演習：Receiving and Routing Data in a Production</a>

    ※ページ内のビデオは日本語切り替えができます。

    <a href="http://github.com/intersystems/Samples-Integration-RedLights" target="_blank">演習内容サンプル</a>
   
- <a href="https://jp.community.intersystems.com/node/483036" target="_blank">【はじめてのInterSystems IRIS】Interoperability（相互運用性）：動作の仕組みを知ろう</a>

- <a href="https://jp.community.intersystems.com/node/483041" target="_blank">【はじめてのInterSystems IRIS】Interoperability（相互運用性）：プロダクションとは</a>

- レコードマップのご紹介

    InterSystems 製品の Interoperability（相互運用性）メニューで使用できるファイル入出力処理に便利な機能をビデオで解説しています。

    {% include youtube-list.html id="dnfPTffiSVo" list="PLzSN_5VbNaxCWpesN3ulh_EZ9sGkw09q5&index=10" %} 
<br>
✅関連記事：<a href="https://jp.community.intersystems.com/node/494326" target="_blank">レコードマップで何ができるか？</a>

- <a href="https://jp.community.intersystems.com/node/483171" target="_blank">【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・プロセス）</a>

- ビジネス・ルールエディタの使い方（※新エディタに未対応）

    {% include youtube-list.html id="4tG-txYZwtg" list="PLzSN_5VbNaxCWpesN3ulh_EZ9sGkw09q5" %}
<br>
>**英語のみとなりますが、以下のオンラインコースもあります。**
>- <a href="https://learning.intersystems.com/course/view.php?name=Integration%20Architecture" target="_blank">オンラインコース（英語）:Integration Architecture</a>
>
>    InterSystems IRIS® data platform、InterSystems HealthShare® の統合機能の基本的なアーキテクチャを学習します。
>    
>   InterSystems の統合ソリューションでは、プロダクションを作成します。このプロダクションには、外部システムと通信する要素とプロダクション内部で処理を実行する要素が含まれます。
>
>   このコースでは、プロダクションの各要素がどのように機能するかを確認します。これらのコンポーネントを通してデータがどのように流れ、システム間の相互運用が可能になるかを学びます。
>
>- <a href="https://learning.intersystems.com/enrol/index.php?id=1426" target="_blank">ビデオ（英語）:Using the Complex Record Mapper</a>
>    
>
>- <a href="https://learning.intersystems.com/enrol/index.php?id=2568" target="_blank">ビデオ（英語）Building BPL Business Processes (1h 30m)</a>
>
>- <a href="https://learning.intersystems.com/enrol/index.php?id=2529" target="_blank">オンラインコース（英語）:Data Transformations Basics</a>
>
>    グラフィカルな管理ポータル・インタフェースを使用して、データ変換を作成する方法を学びます。フィールドをマップする方法、フィールドを変更する関数を使用する方法、およびフィールドの値としてリテラルを使用する方法をご覧ください。最後に、変換をテストして実装する方法を学びます。
>
>    >メモ：変換データとしてHL7を使用しています。
{: .block-tip}

---
## 4. <img src="./assets/icons/4-custom.png" width="70%"/>
FHIR® HL7® V2 コンポーネントなど、多くのビルド済みビジネスコンポーネントが開発者に提供されています。

これだけでは不十分な場合は、カスタムコンポーネントを構築して、データの取り込み方法を完全にカスタマイズすることができます。

- Interoperability メニューで使用するカスタムメッセージクラス作成方法

    ✅ 関連記事：<a href="https://jp.community.intersystems.com/node/483131" target="_blank">【はじめてのInterSystems IRIS】Interoperability（相互運用性）：メッセージ</a>

    {% include youtube.html id="K6jAqSpnaXY"%}

<br>
- <a href="https://jp.community.intersystems.com/node/483136" target="_blank">【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・オペレーション）</a>

- <a href="https://jp.community.intersystems.com/node/483186" target="_blank">【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・サービス）</a>

    アダプタを使用しないビジネス・サービスを直接呼び出す例として REST 経由でのアクセス方法があります。以下、IRIS で REST サーバを作成する方法を解説している関連記事とビデオです。

    ✅ 記事： <a href="https://jp.community.intersystems.com/node/479551" target="_blank">【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：（REST）手動で作成するディスパッチクラス</a>

    ✅ 関連記事：<a href="https://jp.community.intersystems.com/node/559356" target="_blank">REST経由で情報を入力する場合の Interoperability（相互運用性機能）のサンプル</a>

    {% include youtube-list.html id="q3XVT98_05I" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %}

<br>

>**英語のみとなりますが、以下のオンラインコースもあります。**
>- <a href="https://learning.intersystems.com/course/view.php?name=Building%20Custom%20Business%20Operations" target="_blank">オンラインコース（英語）：Building Custom Business Operations</a>
>
>- <a href="https://learning.intersystems.com/course/view.php?id=2574" target="_blank">オンラインコース（英語）：Building Custom Business Services (1h 30m)</a>
>
>- <a href="https://learning.intersystems.com/course/view.php?name=REST%20Services" target="_blank">オンラインコース（英語）：Setting Up RESTful Services</a>
>
>    APIファーストのステップで作る Coffee Maker API
>- <a href="https://learning.intersystems.com/enrol/index.php?id=1716" target="_blank">ビデオ（英語）What is PEX?</a>
>
>    Production EXtension フレームワーク (PEX) を使用すると、ObjectScript を学習することなく .NET または Java でカスタム相互運用性コンポーネントを構築できます。PEX を使用すると使い慣れた言語でコーディングし確立されたコードライブラリを活用してプロダクションにコンポーネントを追加できます。
>
>   PEX を使用してプロダクションを構築する方法については、オンラインコース（英語）<a href="https://learning.intersystems.com/course/view.php?name=PEXInteroperabilityProductions" target="_blank">「Creating Interoperability Productions Using PEX」（1 時間）</a>を受講してください。
{: .block-tip}

---
## 5. <img src="./assets/icons/5-access-multilanguage.png" width="70%"/>

InterSystems IRIS は、各種言語からアクセスすることができます。よくある使い方としては、他 DB と同様に SQL ベースでアクセスする方法があげられます。

このパスの最初に他の SQL データベースからの移行する際よく使用される DDL スクリプトを使用した SQL テーブルを構築する方法について説明します。

{% include youtube.html id="deo8KfS-oeI" %}

<details>
<summary> ▶日本語字幕 </summary>
<div class="transcript">
データベースは、データだけが保存されているのではなくデータを保持するために定義するテーブルやテーブル間のリレーションシップも含まれます。SQL では、データベースの構造を定義および管理するためにデータ定義言語 (DDL) が使用されます。
<br>
DDL スクリプトを使用することでデータベースを InterSystems IRIS data platform に移行したり、既存のデータベースの構造を使用して新しいデータベースを開始したりすることができます。
<br>
全体としてこのプロセスには 2 つの重要なステップがあります。まず、外部データベースまたは InterSystems IRIS から DDL スクリプトをエクスポートします。
<br>
次に、InterSystems Terminal でスクリプトをインポートするコマンドを実行します。InterSystems は、スクリプト内の情報を使用してテーブルとそのリレーションシップを構築します。
<br>
これらの手順を詳しく見ていきましょう。
<br>
まず、DDL スクリプトを作成します。どのデータベース管理システムにも、DDL スクリプトをエクスポートするツールがあります。
<br>
エクスポートされた DDL スクリプトを取得したらそのスクリプトをインポートし InterSystems IRIS でテーブルを作成する ObjectScript コマンドを作成する必要があります。
<br>
InterSystems IRIS の最新バージョンでは、DO $SYSTEM.SQL.Schema.ImportDDL() コマンドを使用します。<br>
続いてメソッドの括弧内に 3 つのパラメータを指定します。最初のパラメータは infile です。インポートする DDL スクリプト・ファイル名のフルパスを記述します。<br>
DDL スクリプトが MSSQL、Sybase、Informix または MySQL で作成された場合は、infile パラメータはリストで指定します。このリストの最初の要素は DDL スクリプトのパスで、その後に TranslateTable の値が続きます。

2 番目のパラメータとして、エラー・ログ・ファイルのフルパス名を指定する logfile を指定します。インポート中にエラーが発生した場合、エラー・テキストがログ・ファイルに保存されます。このパラメータはオプションでなので何も指定しない場合は、デフォルトで 入力ファイル名_Errors.log の名称でログを保存します。
<br>
3 番目のパラメータは DDLMode です。このパラメータには、DDL スクリプトのエクスポートに使用したベンダ (InterSystems IRIS や MySQL など) を入力します。
<br>
DDL スクリプトをインポートする正確なコマンドは、使用している InterSystems IRIS のバージョンによって異なります。InterSystems IRIS バージョン 2020.1 またはそれ以前を使用している場合、コマンドは DO $SYSTEM.SQL.DDLImport() で、3 つの必須パラメータと最大 6 つのオプション・パラメータを引数に指定します。
<br>
DDLMode は最初のパラメータです。
<br>
2 番目のパラメータはもう使用されないので空白のままにしておきます。
<br>
次に infile パラメータ（インポートする DDL スクリプト・ファイルのフル・パス名）です。残りのパラメータはオプションであり、必要に応じてこれらを含めることができます。
<br>
次は、outfileパラメータで、エラーが報告されるファイルのフルパス名を指定します。
<br>
次の 2 つのオプションのパラメータの中の nosup パラメータは、真偽フラグで 1 = TRUE／0 = FALSE のどちらかを指定します。このパラメータを TRUE に設定すると、スクリプトファイルからサポートされていないステートメントが nosupfile に記録されます。
<br>
nosupfile は、デフォルトでは [入力ファイル名_Unsupported.log] の名称でファイルが作成されます。nosupパラメータを FALSE に設定するか、デフォルトのままにすると nosupfile は作成されません。
<br>
nosupfile パラメータの後に、文末区切り文字を指定するパラメータ DEOS を指定します。これは DDL パーサーに 1 つの行がどこで終わり新しい行がどこで始まるかを指示します。DEOS パラメータのデフォルトは、DDLMode　パラメータで指定されたベンダーに基づいた適切な値になります。
<br>
8 番目のパラメータ errpause は、DDL スクリプトの実行中にエラーが発生した場合に InterSystems IRIS が一時停止する秒数です。これが指定されない場合、既定値は 5 秒です。
<br>
最後に、runtimemode パラメータは、DDLMode が InterSystems IRIS の場合にのみ適用され、インポートされた文をどの selectmode で実行するかを指定します： ODBC、DISPLAY、または LOGICAL です。デフォルトでは、LOGICAL モードが使用されます。
<br>
構文は、使用している InterSystems IRIS のバージョンによって異なりますが、コマンドは常に同じ方法で実行され同じ結果を返します。
<br>
InterSystems IRIS Terminal でコマンドを実行します。InterSystems IRIS は、入力ファイルとエラー・ログ・ファイルを返し、インポートされた各 SQL コマンドをリストします。
<br>
エラー・ログ・ファイルは、何も書き込まれていなくても作成されます。InterSystems IRIS 2020.1 以前を使用していてパラメータ nosup を TRUE に設定した場合、サポートされていないログ・ファイルが次にリストされます。このログ・ファイルは、何も書き込まれなくても作成されます。
<br>
DDLスクリプトをインポートしエラーを解決したらデータベースはデータを受け取る準備ができました。
<br>
SQL は ISO/ANSI 標準ですが、独自のコマンドと構文を持つ DDL 言語には多くのバリエーションがあります。InterSystems IRIS 以外からの DDL スクリプトに対応するコマンドの詳細は、InterSystems IRIS ドキュメンテーションの Web サイトを参照してください。
</div>
</details>
<br>
次に、各言語からのアクセス方法について解説します（別のパスに移動します）。

- <a href="JavaApptoISCProducts.html" target="_blank">Java アプリケーションと InterSystems 製品の接続</a>
- <a href="NodeApptoISCProducts.html" target="_balnk">Node.js アプリケーションと InterSystems 製品の接続</a>
- <a href="WritingPythonAppWithInterSystems.html" target="_blank">Python アプリケーションと InterSystems 製品の接続</a>
- <a href="dotNetApptoISCProducts.html" target="_blank">.NET アプリケーションと InterSystems 製品の接続</a>

---
## 6. <img src="./assets/icons/6-APIManagement.png" width="70%"/>

### 1. InterSystems API Managerとは
InterSystems API Manager は、アプリケーション間のゲートウェイとして機能し、トラフィックを監視・制御します。
InterSystems IRIS® データ・プラットフォームと InterSystems IRIS® for Health でどのように機能するのか、また、どのようなシナリオでこの機能が最も有益なのかをご紹介します。

{% include youtube.html id="6oX3HTDI8_A" %}

### 2. InterSystems API Managerのインストール

[ビデオ（英語）:Installing InterSystems API Manager](https://learning.intersystems.com/enrol/index.php?id=1726)

InterSystems API Manager バージョン 1.5+ のインストール手順、InterSystems IRIS® データベース・プラットフォーム・インスタンスとホスト・システムの準備方法、および API Manager インストール・キットで提供されるスクリプトの実行方法について説明します。

### 3. ハンズオン

[演習環境付き演習（英語）:Hands-On with InterSystems API Manager for Developers](https://learning.intersystems.com/course/view.php?name=IAMExercise)

InterSystems API Manager を使用して、InterSystems IRIS® データ・プラットフォーム内のコーヒー・メーカー・アプリケーションの API を管理します。

前提学習または経験 コンテナと Docker の基本的な知識。REST と HTTP リクエスト・レスポンス・ステータス・コードの基礎知識

✅参考記事：[ゼロから使いこなす IAM（InterSystems API Manager）](https://jp.community.intersystems.com/node/493416)

---
## 7. <img src="./assets/icons/7-Analytics.png" width="70%"/>
InterSystems IRISに組み込まれたInterSystems IRIS Business Intelligenceは、ほぼリアルタイムの分析を提供します。このデータを使って、ダッシュボードやピボットテーブルを作成し、スループットを分析したり、規制データを報告したりすることができます。レポート作成に関するリソースは、[「InterSystems Reportsでデータを視覚的に提供する」](#intersystems-reportsでデータを視覚的に提供する)のセクションを参照してください。

- [ビデオ（英語）：InterSystems のアナリティクス入門](https://learning.intersystems.com/course/view.php?id=1979)

    InterSystems®製品のアナリティクス機能をご紹介します
    
    InterSystems IRIS® データ・プラットフォームがサポートする組込みBIとサードパーティツールについて説明し、アナリティクスのニーズに対してこれらのツールをどのように使用できるかを紹介します。
    
    このビデオで説明するコンセプトは、InterSystems IRIS、InterSystems IRIS® for Health、InterSystems Supply Chain Orchestrator™、HealthShare® Health Connectに適用されます。

### InterSystems IRIS BIによるデータ分析

InterSystems IRIS® Business Intelligence に含まれる Analyzer ツールは、データモデルを最大限に活用し、様々な対象者向けに情報を表示する方法を提供します。

このパスでは、InterSystems IRIS® Business Intelligence に含まれる Analyzer ツールを使用して、ピボットテーブルとインタラクティブなダッシュボードを作成し、アプリケーションに組み込んだり、レポートに変換する方法を学習します。

- InterSystems IRIS Business Intelligence 概要

    {% include youtube.html id="xV9Aa31zxhI" %}


- InterSystems Business Intelligenceで使用するキューブ概要

    {% include youtube.html id="xgAdwTy_q1Q" %}


- [ビデオ（英語）:InterSystems IRIS BI: Analyzer](https://learning.intersystems.com/course/view.php?name=IRISBIAnalyzer)

    関連ビデオ：[開発テンプレート（IRIS Analytics Template）の使い方のご紹介（第8回 InterSystems IRIS Analytics コンテスト）](https://jp.community.intersystems.com/node/484826)

    ✅日本語チュートリアル（11シリーズ）：[IRIS BI開発者向けチュートリアルを試してみる](https://jp.community.intersystems.com/node/563396)
    
    ✅[日本語ドキュメント：ダッシュボードの作成](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=D2DASH)

- InterSystems IRIS Business Intelligence：アーキテクト画面の基本の使い方

    {% include youtube.html id="VblJyJl2Xho" %}


### InterSystems IRISのIntegratedMLによる予測

InterSystemsのIRIS®データプラットフォームの機能であるIntegratedMLを使用することで、SQL開発者はアプリケーションのSQLコマンドを使用して予測モデルを構築、トレーニング、実行することができます。

このパスでは、IntegratedML を紹介し、データから予測を開始する方法を紹介します。

- [ビデオ（英語）：機械学習とは](https://learning.intersystems.com/course/view.php?name=What%20is%20ML)

    より深く学習されたい場合は、以下ビデオもご参照ください（日本語）
    {% include youtube-list.html id="47bP5-AtBVU" list="PLzSN_5VbNaxC-z6_DKUZuO__zyudjLE-g" %}

- [インフォグラフィック（英語）:Preparing Your Data for Machine Learning](https://learning.intersystems.com/course/view.php?name=Preparing%20Your%20Data)

    このインフォグラフィックは、データを準備するための基本的なステップと、IntegratedML がそのプロセスをどのように効率化できるかを示しています。データを準備することは、アプリで機械学習を活用するための重要なステップです。

- [インフォグラフィック（英語）:Common Supervised Machine Learning Algorithms](https://learning.intersystems.com/course/view.php?name=Machine%20Learning%20Algorithms)

    ご参考：[機械学習101（2023年11月29日開催　インターシステムズ開発者ウェビナー）](https://www.youtube.com/watch?v=47bP5-AtBVU&list=PLzSN_5VbNaxC-z6_DKUZuO__zyudjLE-g)


- Integrated ML のご紹介～InterSystems IRISのAutoMLご紹介～

    {% include youtube.html id="PFiqENE1uKA" %}


より詳細を確認する場合のおすすめビデオは以下

- SQLから始める機械学習 ～　IntegratedMLのご紹介　～

    {% include youtube-list.html id="3yLK9kBs4ic" list="PLzSN_5VbNaxC-z6_DKUZuO__zyudjLE-g&index=2" %}

- [IntegratedMLとDataRobotの連携](https://www.intersystems.com/jp/integratedml-datarobot-demo/)

- [ビデオ（英語）：IntegratedML: Predicting Readmissions](https://learning.intersystems.com/course/view.php?name=IntegratedMLReadmissions)

- [演習環境付き演習（英語）:Hands-On with IntegratedML](https://learning.intersystems.com/course/view.php?name=HandsOnIntegratedML)

    ✅[機械学習を試せるチュートリアル（日本語）：IntegratedML](https://jp.community.intersystems.com/node/537501)


### InterSystems Reportsでデータを視覚的に提供する

InterSystems IRIS®データ・プラットフォーム、InterSystems IRIS® for Health、HealthShare®でレポートを作成、カスタマイズ、表示するには、InterSystems Reportsを使用します。

- [ビデオ（英語）:Introduction to InterSystems Reports](https://learning.intersystems.com/enrol/index.php?id=1444)

    Logi Analytics が提供する InterSystems Reports は、データのビジュアルレポートを迅速に作成・表示できるレポート作成ツールです。このビデオでは、InterSystems Reports とそのコア・コンポーネントを紹介します。より詳細な情報については、Logi Report のドキュメントをご覧ください。

- [ドキュメント：InterSystems Reports Serverの設定](https://docs.intersystems.com/components/csp/docbook/DocBook.UI.Page.cls?KEY=GISR_server)

- [ドキュメント：Designer Installation](https://docs.intersystems.com/components/csp/docbook/DocBook.UI.Page.cls?KEY=GISR_server)

- [演習環境付き演習（英語）:Getting Started with InterSystems Reports](https://learning.intersystems.com/course/view.php?name=GettingStartedInterSystemsReports) 

    [PDF](https://learning.intersystems.com/course/view.php?name=GettingStartedInterSystemsReports)

- [ビデオ（英語）：Introduction to InterSystems Reports Designer](https://learning.intersystems.com/course/view.php?id=2505)

### アダプティブ・アナリティクスによるデータモデルの構築

InterSystems IRIS® Adaptive Analytics は、AtScale テクノロジーを使用し、Tableau、Excel など、既にお使いのテクノロジーとシームレスに統合することで、セルフサービス型のデータディスカバリー・アナリティクス機能を提供します。

このパスでは、インストールから最初のデータモデルの作成まで、最初の一歩を踏み出す方法をご紹介します。
- ビジネスインテリジェンスにおけるキューブ入門

    {% include youtube.html id="xgAdwTy_q1Q" %}

- [ビデオ（英語）:InterSystems IRIS Adaptive Analytics Overview](https://learning.intersystems.com/course/view.php?id=1754)

    {% include youtube-list.html id="8j6iqmT13XI" list="PLzSN_5VbNaxBlWFxRfrrrScerJrpo7xjr&index=3" %}

- [日本語ドキュメント:InterSystems IRIS Adaptive Analytics](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=AADAN)

- [オンラインコース（英語）：InterSystems IRIS Adaptive Analytics Essential](https://learning.intersystems.com/course/view.php?name=AdaptiveAnalyticsEssentials)

---
## 8. <img src="./assets/icons/8-performance.png" width="70%"/>

アプリケーションのパフォーマンスを必要なだけ確保するためには、高性能なインジェストツールでシステムを構成するだけでなく、大量かつ高速なインジェストのためにシャーディングを設定し、フェイルオーバーのためにミラーリングを設定する必要があります。このセクションでは、これらの推奨事項の多くについて説明する。

- [ビデオ（英語）:InterSystems IRIS Speed Test: High-Volume Ingestion](https://learning.intersystems.com/enrol/index.php?id=1545)

    InterSystems IRIS®データ・プラットフォームの新しいオープン・ソース・ハイブリッド・トランザクション／アナリティカル・プロセッシング（HTAP）スピード・テスト・デモの使用方法をご紹介します。InterSystems IRIS が、リアルタイムのアプリケーション・クエリに答えながら、いかに大量のデータを取り込むことができるかをご覧いただけます。このビデオでは、HTAPスピードテストを使って、InterSystems IRISのパフォーマンスをMySQLやSAP HANAなどの他のデータベースと比較する方法を紹介しています。

- [ビデオ（英語）：Identifying the Benefits of Mirroring and High Availability](https://learning.intersystems.com/course/view.php?id=2338)

- [ビデオ（英語／日本語字幕付き）：Introduction to Sharding in InterSystems IRIS](https://learning.intersystems.com/course/view.php?id=2560)

- [ビデオ（英語／日本語字幕付き）：Planning and Deploying a Sharded Cluster](https://learning.intersystems.com/course/view.php?id=2586)

- [ビデオ（英語）：Finding and Fixing Slow SQL Queries](https://learning.intersystems.com/course/view.php?id=2422)

- [体験環境付き演習（英語）：Optimizing SQL Queries in InterSystems IRIS](https://learning.intersystems.com/course/view.php?id=2533)

    トレーニングコースで同様の内容をご確認いただけます。

    ✅対応するコース：[InterSystems SQL](https://www.intersystems.com/jp/intersystems-sql/)
