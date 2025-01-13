---
title: FHIRアプリケーション構築の基礎
date: 2024-12-03
permalink: BuildingBasicFHIRIntegration.html
layout: post
---
>オリジナル：[Building Basic FHIR Integrations with InterSystems](
https://learning.intersystems.com/course/view.php?id=1959)

このパスでは、InterSystems IRIS for Health™ または HealthShare® Health Connect を使用して HL7® FHIR® アプリケーションを構築するための基本を学習します。

最初にFHIR エンドポイントを設定し、FHIR リソースの入力や変換方法を学習します。また、API を管理し、クライアントアプリケーションから FHIR リソースを参照する方法も学習します。

はじめて FHIR について学習する方は、[HL7 FHIRとは](IntroFHIRStandard.html)からはじめてみてください。

InterSystems製品を利用したシステム統合処理についての前提知識を確認される場合は以下コンテンツをご利用ください。

- InterSystems製品の基本構造について

    ✅ 記事：[【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その2：InterSystems IRIS で開発をはじめよう！](https://jp.community.intersystems.com/node/478601)

    {% include youtube-list.html id="ID6ImJTgJRk" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ&index=3" %}

- InterSystems Interoperability(相互運用性)概要を確認する

    以下のビデオの12分以降をご覧ください。

    {% include youtube-list.html id="vo12UnH-c-s" list="PLzSN_5VbNaxD-r8wU4LHwLwGSzUjrffEX&index=1&t=1203s" %}

- InterSystems Interoperability（相互運用性）をサンプルコードを見ながら学習する

    ✅ シリーズ記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）を使ってみよう！](https://jp.community.intersystems.com/node/483021)

    ✅ シリーズ記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：動作の仕組みを知ろう](https://jp.community.intersystems.com/node/483036)

    ✅ シリーズ記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：プロダクションとは](https://jp.community.intersystems.com/node/483041)


> **英語のオンラインコースもあります**
>- [オンラインコース（英語）：Integration Architecture（英語）](https://learning.intersystems.com/course/view.php?name=Integration%20Architecture)
{: .block-tip}

---

[1. <img src="./assets/icons/FHIR/Integration1.png" width="40%"/>](#1-)

[2. <img src="./assets/icons/FHIR/Integration2.png" width="40%"/>](#2-)

[3. <img src="./assets/icons/FHIR/Integration3.png" width="40%"/>](#3-)

[4. <img src="./assets/icons/FHIR/Integration4.png" width="40%"/>](#4-)

[5. <img src="./assets/icons/FHIR/Integration5.png" width="40%"/>](#5-)

[6. <img src="./assets/icons/FHIR/Integration6.png" width="40%"/>](#6-)

[7. <img src="./assets/icons/FHIR/Integration7.png" width="40%"/>](#7-)

---
## 1. <img src="./assets/icons/FHIR/Integration1.png" width="70%"/>

最初に、医療用文書の標準フォーマットとして、また医療相互運用性にとってFHIRが重要である理由を学び、InterSystems IRIS for HealthがどのようにFHIRインテグレーションとアプリケーション開発をサポートしているかを確認しましょう。


- ビデオ（日本語）：HL7® FHIR® × InterSystems IRIS for Health(https://www.youtube.com/watch?v=rbIF4z8xRIY&list=PLzSN_5VbNaxBu4kMgZrK5iGi-GIGNxvpu&index=1)

    {% include youtube-list.html id="rbIF4z8xRIY" list="PLzSN_5VbNaxBu4kMgZrK5iGi-GIGNxvpu&index=1" %}

- ビデオ（日本語字幕）:FHIR - 未来のために設計された医療データスタンダード "FHIR A Healthcare Data Standard Designed for the Future"

    {% include youtube.html id="gNjlaARboYk" %}

- [ドキュメント：FHIRサーバー：アーキテクチャ](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=HXFHIR_server_arch)

> **英語ビデオもあります**
>- [What is FHIR？](https://learning.intersystems.com/course/view.php?n―me=What%20is%20FHIR)
{: .block-tip}

---
## 2. <img src="./assets/icons/FHIR/Integration2.png" width="70%"/>

IRIS for Health は、FHIR データを格納する FHIR エンドポイントを作成でき、他の FHIR プロファイルをサポートするように構成することができます。

InterSystems IRIS for Health が受信する HL7® CDA®、CSV、HL7® V2、XML データを FHIR フォーマットに変換する方法をご覧ください。

- [ドキュメント：FHIR サーバのインストールと構成](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=HXFHIR_server_install)

- [演習環境付き体験（英語）：Importing FHIR Packages into the InterSystems IRIS for Health Server](https://learning.intersystems.com/course/view.php?id=1721)


✅ ビデオ：他形式データからFHIR への変換

{% include youtube-list.html id="dsB3cS333LI" list="PLzSN_5VbNaxBu4kMgZrK5iGi-GIGNxvpu&index=9" %}

✅ ビデオ：FHIR プロファイル(https://jp.community.intersystems.com/node/495321)

{% include youtube-list.html id="B-B6ge_0nHg" list="PLzSN_5VbNaxBu4kMgZrK5iGi-GIGNxvpu&index=8" %}


✅ [FHIR R4 リソースリポジトリを簡単にお試しいただける開発環境テンプレートのご紹介](https://jp.community.intersystems.com/node/491836)

✅ ビデオ：REST クライアントから FHIR R4 リソースリポジトリにアクセスする例

{% include youtube-list.html id="AYz6d7MxXos" list="PLzSN_5VbNaxBu4kMgZrK5iGi-GIGNxvpu&index=11" %}



---
## 3. <img src="./assets/icons/FHIR/Integration3.png" width="70%"/>

InterSystems IRIS for Health を使用して、Summary Document Architecture（SDA）と組み込みの変換を使用して、受信データを FHIR フォーマットに変換します。

> **英語ビデオやオンラインコース**
>- [ビデオ（英語）：Converting Legacy Data to HL7 FHIR R4 in InterSystems IRIS for Health](https://learning.intersystems.com/course/view.php?id=1744)
>
>- [ビデオ(英語)：What is SDA?](https://learning.intersystems.com/course/view.php?id=2128)
>
>- [オンラインコース(英語)：Transforming Data into the HL7 FHIR Format](https://learning.intersystems.com/course/view.php?id=2149)
>
>    InterSystems IRIS for Health™ または HealthShare® Health Connect を使用して、医療システム間のデータ交換に一般的に使用されている HL7® FHIR® フォーマットにデータを変換する方法をお試しいただけます。
>    
>    また、後半では、ダイナミックオブジェクトを使用して FHIR データを操作する方法を学びます。このコースを通して、HL7 V2 リソースを FHIR フォーマットに変換する方法を体験できます。
{: .block-tip}


✅ この他に、InterSystems の内部形式であるSDAを使用せず、[JSONTemplateエンジン](https://github.com/Intersystems-jp/JSONTemplate)を使い、FHIRリソースのような複雑なJSONフォーマットを簡単に生成する方法も用意しています。

> **このテンプレートエンジンは、FHIRに限らず複雑なJSONフォーマットを生成するのに役立つエンジンです。**
>
>参考記事：[複雑なJSONの生成に便利な「JSONテンプレートエンジン」の使い方ご紹介](複雑なJSONの生成に便利な「JSONテンプレートエンジン」の使い方ご紹介)
{: .block-tip}

JSONテンプレートエンジンを利用して FHIR リソースの JSON を生成される方法については、以下ビデオで説明しています。

{% include youtube-list.html id="H4LzOV-Tfzg" list="PLzSN_5VbNaxB39_H2QMMEG_EsNEFc0ASz" %}


- 講師付きトレーニングコースで使用している[CSVからFHIRリソースを作成するFHIRファサード](https://github.com/iijimam/Training-FHIRFacadeEx)のサンプルコードを公開しています。

    JSONテンプレートエンジンを利用して、どのようにCSVから FHIR リソース変換しているか、については、[README](https://github.com/iijimam/Training-FHIRFacadeEx/blob/master/readme.md)をご参照ください。

> **上記内容をカバーする講師付きトレーニングもご提供しています**
>- CSVからFHIRへの変換
>    
>    JSONテンプレートエンジンを利用した変換方法を習得できるコースです。
    作成例として、CSVで入力された情報からFHIRリソースを作成し、IRISに用意したFHIRリポジトリに登録する流れを体験します。
>
>- SSMIX2からFHIRへの変換（これは掲載する？）
>
>    SDA経由の変換を体験できるコースです。
>
> 教育サービス担当まで下記ページ末尾のお問い合わせフォームからご依頼ください。
> [問い合わせフォーム](https://www.intersystems.com/jp/course-offerings/)
{: .block-warning}

---
## 4. <img src="./assets/icons/FHIR/Integration4.png" width="70%"/>

CRUDインタラクションの実行-クライアントアプリケーションからの FHIR リソースの検索や、RESTクライアントからの操作のテストなどを確認できます。

- 日本語ビデオ：FHIR+IRIS for Health 101（18分ごろからご覧ください）

{% include youtube-list.html id="S7PV3RIpMUM" list="PLzSN_5VbNaxBu4kMgZrK5iGi-GIGNxvpu&index=10&t=1077" %}


- [ドキュメント：相互作用（インタラクション）](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=HXFHIR_server_arch_supported_interactions)

> **英語ビデオもあります**
>- [ビデオ：Searching for FHIR Resources in InterSystems IRIS for Health](https://learning.intersystems.com/course/view.php?id=1287)
{: .block-tip}

---
## 5. <img src="./assets/icons/FHIR/Integration5.png" width="70%"/>
新しい FHIR サーバーをセットアップする際に、OAuth2.0でエンドポイントを保護する方法を学習します。

- [ドキュメント：OAuth2.0認証](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=HXFHIR_server_auth_oauth)

- [ドキュメント（英語）：OAuth FHIR Client Quickstart](https://docs.intersystems.com/irisforhealth20243/csp/docbook/DocBook.UI.Page.cls?KEY=HXFHIR_server_auth#HXFHIR_server_auth_oauth)

    InterSystems サーバーに用意する FHIR リソースサーバーと OAuth 2.0 認証サーバーの接続のための設定を簡単に作成する方法も用意されています（バージョン2025.1以降）


- [ビデオ（英語）：Configuring the InterSystems Web Gateway](https://learning.intersystems.com/course/view.php?id=1787)


---
## 6. <img src="./assets/icons/FHIR/Integration6.png" width="70%"/>

InterSystems API Manager を使用して FHIR エンドポイントへのトラフィックを制御する方法と、トラブルシューティングのテクニックを紹介します。

- [ゼロから使いこなす IAM（InterSystems API Manager）](https://jp.community.intersystems.com/node/493416)

> **英語ビデオもあります**
>
>- [ビデオ：What is InterSystems API Manager](https://www.youtube.com/watch?v=XI1oqKEwLL0)
{: .block-tip}

- [体験環境付き演習（英語）：Building FHIR Applications with InterSystems API Manager](https://learning.intersystems.com/course/view.php?id=1654)

    ✅ [演習資料PDF](https://learning.intersystems.com/pluginfile.php/38823/mod_resource/content/10/FHIRExerciseGuide%20%281%29.pdf)

    InterSystems API Manager を使用して API を表示し、HL7® FHIR® アプリケーションを作成して、FHIR リクエストを監視する方法について説明します。

    この実習を修了するまでに、以下のことができるようになります：

    - InterSystems API Manager を使用して API を表示し、FHIR 要求のテスト
    - REST クライアントを使用して、InterSystems IRIS for Health™ に FHIR リクエストを作成
    - FHIR アプリケーションを InterSystems IRIS for Health に接続させる
    - API Manager 開発者ポータルで統計を表示して API 呼び出しを監視

- [ドキュメント：FHIR サーバのデバッグ](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=HXFHIR_server_debugMaintain)


---
## 7. <img src="./assets/icons/FHIR/Integration7.png" width="70%"/>

最後の演習では、サンプルのフロントエンドを使って、完全な FHIR アプリケーションを構築するします。

- [体験環境付き演習（英語）：Working with the FHIR Resource Repository](https://learning.intersystems.com/course/view.php?name=FHIR%20Resource%20Repository)

    Syntheaデータ入れてRESTクライアントからのアクセスを試します。また、簡単な Web ページwを利用して、FHIRリポジトリからの検索結果を表示させる内容を体験できます。
    

> **[FHIR R4 リソースリポジトリを簡単にお試しいただける開発環境テンプレートのご紹介](https://jp.community.intersystems.com/node/491836) で提供しているコンテナ環境を利用して同様の内容をお試しいただけます。**
{: .block-warning}
