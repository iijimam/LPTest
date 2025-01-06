---
title: インプリメンテーションパートナ向けInterSystems製品をはじめよう！
date: 2024-12-02
permalink: /GettingStarted-ImplePartner-All.html
---

InterSystems IRIS® データプラットフォームを利用して開発するアプリケーションに必要となるコードの記述、インテグレーションの構築、コンポーネントの作成方法、また利用可能なツールについて学習します。

この学習プログラムは、InterSystems IRISを初めて導入する方を対象としています。

> パートナーになることに興味がありますか？[インプリメンテーション・パートナー・プログラムの詳細](https://www.intersystems.com/jp/partners/implementation-partners/)をご覧ください。


このラーニング・パスを終了することに加え、以下の講師付きクラスルームトレーニングコースに参加／個別開催の申し込みを行うことを強く推奨します。

- [InterSystems SQL](https://www.intersystems.com/jp/intersystems-sql/)
- [InterSystems Object](https://www.intersystems.com/jp/intersystems-object/)
    - このコースは**ObjectScriptを学習するコースではありません。**
    - InterSystems製品でオブジェクト指向プログラミングを行う方法、また永続クラス定義の作成、オブジェクト操作方法を学習するためのコースです。
- [InterSystems Server システム管理1](https://www.intersystems.com/jp/intersystems-server-system-administration/)
- [InterSystems Server システム管理2：セキュリティ管理編](https://www.intersystems.com/jp/intersystems-server-system-administration-2/)

---
学習順序は以下の通りです。
1. <img src="./assets/icons/IRIS.png" width="10%"/>[InterSystems IRIS とは？](#1-intersystems-iris-とは)
2. <img src="./assets/icons/serversideapp-better-dicision.png" width="10%"/>[サーバサイドアプリケーションの構築](#2-サーバーサイドアプリケーションの構築)
3. <img src="./assets/icons/integration.png" width="10%"/>[他のシステムとの統合](#3-他のシステムとの統合)
4. <img src="./assets/icons/custom.png" width="10%"/>[カスタムコンポーネントを使用したシステム統合の開発](#4-カスタムコンポーネントを使用したシステム統合の開発)
5. <img src="./assets/icons/access-multilanguage.png" width="10%"/>[他言語を使用したデータアクセス](#5-他言語を使用したデータアクセス)
6. <img src="./assets/icons/APIManagement.png" width="10%"/>[APIの管理](#6-apiの管理)
7. <img src="./assets/icons/Analytics.png" width="10%"/>[データ分析](#7-データ分析)
8. <img src="./assets/icons/performance.png" width="10%"/>[パフォーマンスとスピードの最適化](#8-パフォーマンスとスピードの最適化)

---


## <img src="./assets/icons/IRIS.png" width="10%"/>1. InterSystems IRIS とは？

InterSystems IRIS®データ・プラットフォームは、信頼性の高い統一プラットフォームで、重要なアプリケーションを迅速に開発・デプロイすることを可能にします。

- InterSystems IRISとは（日本語字幕入りビデオ）

    {% include youtube.html id="w2OeWx3WNOs" %}


> **もう少し詳しく確認されたい方は約30分の以下ビデオをご参照ください。**
>
>- InterSystems IRIS データプラットフォームのご紹介    
>    
>{% include youtube-list.html id="vo12UnH-c-s" list="PLzSN_5VbNaxD-r8wU4LHwLwGSzUjrffEX" %}
{: .block-tip}


- InterSystems へようこそ

    {% include youtube.html id="v4uoejre5IU" %}

---
## <img src="./assets/icons/serversideapp-better-dicision.png" width="10%"/>2. サーバーサイドアプリケーションの構築

InterSystems 製品の組み込み言語である InterSystems ObjectScript を使用して、新しいクラスの作成、オブジェクトの操作、SQL クエリの実行について学習します。

このパスを終了すると、ObjectScript を使用してInterSystems製品のサーバーサイド・アプリケーションを構築することができるようになり、以下の開発に役立てることができます。

- データ操作以外の処理も含めたストアドプロシージャの開発
- Interoprabilityで使用するカスタム・ビジネス・コンポーネントの開発
- ビジネスルールとメッセージルータのコードで作成するカスタム関数
- カスタムコードによる高度なデータ変換の作成

カスタム・ビジネス・コンポーネントの構築方法の詳細については[「カスタムコンポーネントを使用したシステム統合の開発」](#4-カスタムコンポーネントを使用したシステム統合の開発)をご参照ください。

### はじめに

最初に、概要をビデオでご覧ください。その後、InterSystems IRIS® データプラットフォームのアーキテクチャとクラスの基本を学び、ObjectScript でのコーディングを開始します。

- InterSystems 製品のアーキテクチャ概要 ～ネームスペースとデータベース～

    {% include youtube-list.html id="TNjUnuw8K_Q" list="PLzSN_5VbNaxCWpesN3ulh_EZ9sGkw09q5" %} 


### 日本語：セルフラーニングビデオ

オリエンテーションに最適なセルフラーニングビデオやコンテンツをご用意しています。

- 以下動画から、IRISの開発環境の作成方法、ネームスペース／データベースについて、IDEからIRISに接続する方法を確認できます。

    ✅ [【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その2：InterSystems IRIS で開発をはじめよう！](https://jp.community.intersystems.com/node/478601)

    {% include youtube-list.html id="ID6ImJTgJRk" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %} 
    

- ObjectScriptの基本操作の学習については、**[ObjectScript クックブック：ObjectScriptの基本のき！](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/Basic.md)** をご参照ください。

- 以下動画から、クラス定義の作成からインスタンス生成、保存までの流れを確認できます。

    ✅ [【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その3：IRIS でクラス定義を作ろう（オブジェクト操作の練習）](https://jp.community.intersystems.com/node/478606)

    {% include youtube.html id="kWJCzn9bndQ" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %} 


- 以下動画からInterSystems製品でのJSON操作方法をご確認いただけます。

    ✅ コピペ元がある記事：[【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：IRIS での JSON の操作](https://jp.community.intersystems.com/node/480106)

    {% include youtube-list.html id="045HRug72VE" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %} 


- メソッド内でSQLを記述する方法については、以下クックブックをご参照ください。

    ✅ [ObjectScriptクックブック：7.メソッドやルーチンでSQLを実行する方法](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/Basic.md#7-%E3%83%A1%E3%82%BD%E3%83%83%E3%83%89%E3%82%84%E3%83%AB%E3%83%BC%E3%83%81%E3%83%B3%E3%81%A7sql%E3%82%92%E5%AE%9F%E8%A1%8C%E3%81%99%E3%82%8B%E6%96%B9%E6%B3%95)


関連するトレーニングコースは以下の通りです。
- [InterSystems Object（2日間）](https://www.intersystems.com/jp/intersystems-object/)
- [InterSystems SQL（2日間）](https://www.intersystems.com/jp/intersystems-sql/)
  

> **英語のみとなりますが、以下のオンラインコースもあります。**
>
> - [オンラインコース（英語）：Creating an InterSystems Class Definition in VS Code](https://learning.intersystems.com/course/view.php?name=IRIS%20Class)
>
> - [オンラインコース（英語）:InterSystems ObjectScript Basics](https://learning.intersystems.com/course/view.php?name=Cach%C3%A9%20ObjectScript%20Basics)
>
> - [オンラインコース（英語）:InterSystems IRIS Objects Introduction](https://learning.intersystems.com/enrol/index.php?id=2225)
>
> - [オンラインコース（英語）：InterSystems SQL Overview](https://learning.intersystems.com/enrol/index.php?id=960)
>
> - [オンラインコース（英語）:Using JSON in InterSystems IRIS](https://learning.intersystems.com/course/view.php?name=JSON%20in%20IRIS)
>
> - [演習環境付き演習（オンラインコース）：Learning Path Exercise: Building a Server-Side Application with InterSystems IRIS](https://learning.intersystems.com/course/view.php?name=Server-Side%20Application%20Exercise)
>
>    InterSystems IRIS® データプラットフォームと InterSystems ObjectScript を使用して、小規模なデータベースアプリケーションを作成します。
>    
>    この演習では、InterSystems IRIS を使用したサーバサイド・アプリケーションの構築の学習パスで学習したすべてのスキルを結集して、大規模な書籍コレクションに関する情報を格納および取得するためのクラスを作成し、SQL を使用します。
>    
>    この演習は、既存の知識をテストするために学習パスを開始する前に、またはキャップストーン・プロジェクトとして最後にお試しください。
{: .block-tip}


### 認定テスト受験の準備が整ったら・・・

インターシステムズ・ラーニング・サービスは、業界標準の認定試験を提供し、あなたがインターシステムズの技術を習得していることを証明します。当社の試験は、安全なオンライン試験監督とセルフサービス予約で提供されます。受験者は、いつでもどこでも、都合のよいときに試験を受けることができます。

※英語のみ：[Exam: InterSystems IRIS Core Solutions Developer Specialist](https://www.intersystems.com/education/)


---
## <img src="./assets/icons/integration.png" width="10%"/>3. 他のシステムとの統合

インターシステムズ製品のInteroperability(相互運用性)フレームワークにより、インターフェイスエンジニアやソフトウェア開発者は、複数のシステムを接続し、下流のアプリケーションにメッセージを迅速にルーティングすることができます。

このパスでは、インテグレーションの基本を学び、組み込みオプションとカスタムオプションを使用してデータを送信、受信、処理、変換する方法を確認します。

- [体験環境付き演習：Receiving and Routing Data in a Production](https://learning.intersystems.com/course/view.php?name=Interop%20QS)

    ※ページ内のビデオは日本語切り替えができます。

    演習内容サンプルはこちら👉http://github.com/intersystems/Samples-Integration-RedLights
   
- [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：動作の仕組みを知ろう](https://jp.community.intersystems.com/node/483036)

- [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：プロダクションとは](https://jp.community.intersystems.com/node/483041)

- レコードマップのご紹介

    InterSystems製品のInteroperability（相互運用性）メニューで使用できるファイル入出力処理に便利な機能をビデオで解説しています。

    {% include youtube-list.html id="dnfPTffiSVo" list="PLzSN_5VbNaxD-r8wU4LHwLwGSzUjrffEX" %} 


✅関連記事：[レコードマップで何ができるか？](https://jp.community.intersystems.com/node/494326)


- [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・プロセス）](https://jp.community.intersystems.com/node/483171)

- ビジネス・ルールエディタの使い方（※新エディタに未対応）

    {% include youtube-list.html id="4tG-txYZwtg" list="PLzSN_5VbNaxCWpesN3ulh_EZ9sGkw09q5" %}

>**英語のみとなりますが、以下のオンラインコースもあります。**
>- [オンラインコース（英語）:Integration Architecture](https://learning.intersystems.com/course/view.php?id=908)
>
>    InterSystems IRIS®データプラットフォーム、InterSystems HealthShare®、InterSystems Ensemble®の統合機能の基本的なアーキテクチャを学習します。
>    
>    これらのコンポーネントを通じてデータがどのように流れ、システム間の相互運用が可能になるかを学びます。
>
>    このコースには、3 つのレッスンと数問のクイズが含まれています。ビデオはフルスクリーンモードでご覧ください。
>
>- [ビデオ（英語）:Using the Complex Record Mapper](https://learning.intersystems.com/enrol/index.php?id=1426)
>    
>
>- [ビデオ（英語）Building BPL Business Processes (1h 30m)](https://learning.intersystems.com/enrol/index.php?id=2030)
>
>- [オンラインコース（英語）:Data Transformations Basics](https://learning.intersystems.com/enrol/index.php?id=1170)
>
>    グラフィカルな管理ポータル・インタフェースを使用して、データ変換を作成する方法を学びます。フィールドをマップする方法、フィールドを変更する関数を使用する方法、およびフィールドの値としてリテラルを使用する方法をご覧ください。最後に、変換をテストして実装する方法を学びます。
>
>    >メモ：変換データとしてHL7を使用しています。
{: .block-tip}

---
## <img src="./assets/icons/custom.png" width="10%"/>4. カスタムコンポーネントを使用したシステム統合の開発
FHIR® HL7® V2 コンポーネントなど、多くのビルド済みビジネスコンポーネントが開発者に提供されています。

これだけでは不十分な場合は、カスタムコンポーネントを構築して、データの取り込み方法を完全にカスタマイズすることができます。

- Interoperabilityメニューで使用するカスタムメッセージクラス作成方法

    関連記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：メッセージ](https://jp.community.intersystems.com/node/483131)

    {% include youtube.html id="K6jAqSpnaXY"%}


- [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・オペレーション）](https://jp.community.intersystems.com/node/483136)

- [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・サービス）](https://jp.community.intersystems.com/node/483186)

    アダプタを使用しないビジネス・サービスを直接呼び出す例としてREST経由でのアクセス方法があります。以下、IRISでRESTサーバを作成する方法を解説している関連記事とビデオです。

    ✅ 記事： [【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：（REST）手動で作成するディスパッチクラス](https://jp.community.intersystems.com/node/479551)

    ✅ 関連記事：[REST経由で情報を入力する場合の Interoperability（相互運用性機能）のサンプル](https://jp.community.intersystems.com/node/559356)

    {% include youtube-list.html id="q3XVT98_05I" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %}

    

>**英語のみとなりますが、以下のオンラインコースもあります。**
>- [オンラインコース（英語）：Building Custom Business Operations](https://learning.intersystems.com/course/view.php?name=Building%20Custom%20Business%20Operations)
>
>- [オンラインコース（英語）:Building Custom Business Services (1h 30m)](https://learning.intersystems.com/enrol/index.php?id=2031)
>
>- [オンラインコース（英語）:Setting Up RESTful Services](https://learning.intersystems.com/course/view.php?name=REST%20Services)
>
>    APIファーストのステップで作るCoffee Maker API
>- [ビデオ（英語）What is PEX?](https://learning.intersystems.com/enrol/index.php?id=1716)
>
>    Production EXtension フレームワーク (PEX) を使用すると、ObjectScript を学習することなく、.NET または Java でカスタム相互運用性コンポーネントを構築できます。PEX を使用すると、使い慣れた言語でコーディングし、確立されたコードライブラリを活用して、プロダクションにコンポーネントを追加できます。PEX を使用してプロダクションを構築する方法については、オンラインコース（英語）[「Creating Interoperability Productions Using PEX」（1 時間）](https://learning.intersystems.com/course/view.php?name=PEXInteroperabilityProductions)を受講してください。
{: .block-tip}

---
## <img src="./assets/icons/access-multilanguage.png" width="10%"/>5. 他言語を使用したデータアクセス

InterSystems IRIS は、各種言語からアクセスすることができます。よくある使い方としては、他DBと同様にSQLベースでアクセスする方法があげられます。

このパスの最初に、他の SQL データベースからの移行する際、よく使用される DDL スクリプトを使用した SQL テーブルを構築する方法について説明します。

[ビデオ（英語）Importing Relational Data Using a DDL Script](https://learning.intersystems.com/course/view.php?id=2174)

次に、各言語からのアクセス方法について解説します。

### Connecting Java Applications to InterSystems Products

#### 1. はじめに

あなたの好みの API を使用して、Java アプリケーションを InterSystems IRIS® データプラットフォームやその他のインターシステムズ製品およびテクノロジに接続します。（APIは、JDBC、XEP、Hibernate、Native APを選択できます）

- [ビデオ（英語／日本語字幕あり）Java Overview](https://learning.intersystems.com/course/view.php?name=Java%20Overview)

- [ビデオ（英語）Using a Java Shared Memory Connection](https://learning.intersystems.com/course/view.php?name=Shared%20Memory%20Connection)

#### 2. JDBC経由でテーブルにアクセスする

- [ビデオ（英語／日本語字幕あり）Using JDBC with InterSystems IRIS](https://learning.intersystems.com/enrol/index.php?id=881)

- [ドキュメント：InterSystems IRIS デモ ： JDBC とインターシステムズのデータベース](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=AFL_jdbc)

### Connecting Node.js Applications to InterSystems Products

ODBC または InterSystems IRIS® データプラットフォームのNative API を使用して、Node.js アプリケーションを InterSystems® 製品およびテクノロジーに接続できます。

#### 1. はじめに
Node.js の概要と、InterSystems ODBC ドライバ、および Node.js のネイティブ API について紹介します。

- [ビデオ（英語／日本語字幕あり）Node.js Overview](https://learning.intersystems.com/course/view.php?id=1105)

- [ドキュメント：はじめに ： インターシステムズ・データベースへの ODBC 接続](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BNETODBC_intro)

- [ドキュメント：Native SDK for Node.js の概要](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BJSNAT_intro)

#### 2. ODBC経由でIRISにアクセスする

- [ドキュメント：Node.js リレーショナル・アクセスのサポート](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BNETODBC_support#BNETODBC_support_nodeodbc)

#### 3. Native APIの低レイテンシー機能を利用する

- [体験環境付き演習（英語のみ）：Stock Trading with Node.js](https://learning.intersystems.com/course/view.php?id=2597)


### Writing Python Applications with InterSystems
既存の Python コーディングスキルを活用して、InterSystems® アプリケーションを強化します。

クライアントの Python アプリケーションを接続する方法、InterSystems ObjectScript コードに Python を組み込む方法、あるいは、Python ライブラリの呼び出しに重い処理が必要な場合に別のサーバを使用して呼び出しを最適化する方法について説明します。

#### 事前準備
Pythonの基本的なコーディング経験があることを前提としています。[Python for Beginers](https://www.python.org/about/gettingstarted/)も併せてご参照ください。

#### 1. はじめに
InterSystemsのアプリケーションで Python ライブラリを活用する方法をご確認いただけます。

pyodbc を使用して既存の Python アプリケーションを接続したり、Embedded Python を使用して Python と ObjectScript を並行してコーディングすることができます。また、InterSystems Native API または外部言語サーバを使用して、Python で完全な InterSystems アプリケーションを構築することもできます。

[Overview of Python in InterSystems Products (1m)](https://learning.intersystems.com/mod/page/view.php?id=11611)

#### 2. クライアントのPythonアプリケーションからIRISへ接続する

Python アプリケーションをインターシステムズ製品に接続するための最も一般的なオプションである pyodbc の使用方法について説明します。

ドキュメント：[pyodbc Python ODBC ブリッジのサポート](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BNETODBC_support_pyodbc)


#### 3. PythonをObjectScriptと並行して実行する
Embedded Pythonを使用して、ObjectScriptと並行してPythonライブラリを呼び出す方法を解説します。

- [日本語字幕付：What Is Embedded Python?](https://learning.intersystems.com/course/view.php?name=EmbeddedPythonOverview)

- [体験環境付き演習：Embedded Python QuickStart](https://learning.intersystems.com/course/view.php?name=EmbeddedPythonQS)

    ※ビデオは日本語字幕に切り替えができます。

- [体験環境付き演習：Parsing Images and Charting Data with Embedded Python](https://learning.intersystems.com/course/view.php?id=2604)

    同じ内容ではありませんが、サンプルコード付きの日本語記事もあります。

    ✅[Embedded Python を使ってレシート（JPG）の中身を IRIS に登録してみました](https://jp.community.intersystems.com/node/513136)


**💡日本語のセルフラーニングビデオのプレイリストはこちら**（記事はこちら[【はじめてのInterSystems IRIS】Embedded Python セルフラーニングビデオシリーズ公開！](https://jp.community.intersystems.com/node/520751)）

- Embedded Python 概要編

    {% include youtube-list.html id="QYbglSZljzs" list="PLzSN_5VbNaxBowDUZQfqL3bvaXpkCMPW2&index=1"%}

- Embedded Python 利用前の準備

    {% include youtube-list.html id="frOsOK_T4UI" list="PLzSN_5VbNaxCqdcK4yiFwzXe041RBtD6V" %}


- Embedded Pythonでデータベースプログラミング：SQLアクセス編

    {% include youtube-list.html id="oDgKd5FTq2k" list="PLzSN_5VbNaxDAPjSBe5F-uGbGkoJqcerL" %}

- Embedded Pythonでデータベースプログラミング：オブジェクトアクセス編

    {% include youtube-list.html id="9M_WFS8LPQM" list="PLzSN_5VbNaxBnEb5rq-676b1l7Ym6INjL" %}

- IRISでPythonを使ってみよう（Embedded Python）

    {% include youtube.html id="HFq-IIlejMg" list="PLzSN_5VbNaxBLXlC9oCgwPtxBilT8tJ96" %}


#### 4. PythonでInterSystems IRISアプリケーションを構築する

InterSystems Python SDK を使用して、Python から InterSystems IRIS クラスのインスタンスをリモートで作成および操作できます。 また、外部言語サーバを使用して、InterSystems 製品から外部プロセスで実行されている Python コードを呼び出す方法をご確認いただけます。

- [ビデオ（英語）Using the Native API for Python](https://learning.intersystems.com/course/view.php?name=Native%20API%20for%20Python)

- [体験環境付き演習：Embedded Python QuickStart](https://learning.intersystems.com/course/view.php?name=EmbeddedPythonQS)

- [ドキュメント：外部言語の操作](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BEXTSERV_coding)

- [体験環境付き演習：Interacting with Data in Python Using Multiple Data Models](https://learning.intersystems.com/course/view.php?name=PythonMultiModel)

- [ビデオ（英語）：Evaluating Python Development Strategies](https://learning.intersystems.com/course/view.php?id=2063)

---
## <img src="./assets/icons/APIManagement.png" width="10%"/>6. APIの管理

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
## <img src="./assets/icons/Analytics.png" width="10%"/>7. データ分析
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
## <img src="./assets/icons/performance.png" width="10%"/>8. パフォーマンスとスピードの最適化

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
