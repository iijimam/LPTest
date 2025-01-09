---
title: FHIR - InterSystems IRIS for Healthでアプリケーションを有効にする
date: 2024-12-02
permalink: FHIR-EnablingYourAppWithIRIS4H.html
layout: post
---

> オリジナル[FHIR-Enabling Your Applications with InterSystems IRIS for Health](https://learning.intersystems.com/course/view.php?id=2323)

InterSystems IRIS for Health™ を使用して、FHIR ファサード を作成し、ヘルスケア・アプリケーションが HL7® FHIR® フォーマットでデータを送受信できるようにすることができます。このラーニングパスでは、以下の方法を学習します。

- RESTを使用して、EHRのような外部のFHIRサーバーと対話するようにアプリケーションをセットアップする。
- 標準的なヘルスケアデータ形式のメッセージを FHIR 形式に変換する。
- FHIR Interoperability Adapterを使用してFHIR ファサードを設定する。


[1. <img src="./assets/icons/FHIR/Second1.png" width="40%"/>](#1-)

[2. <img src="./assets/icons/FHIR/Second2.png" width="40%"/>](#2-)

[3. <img src="./assets/icons/FHIR/Second3.png" width="40%"/>](#3-)

[4. <img src="./assets/icons/FHIR/Second4.png" width="40%"/>](#4-)

[5. <img src="./assets/icons/FHIR/Second5.png" width="40%"/>](#5-)

---
## 1. <img src="./assets/icons/FHIR/Second1.png" width="70%"/>

FHIRの基本的な知識について確認するため、以下のビデオをご参照ください。

このビデオは、国際モダンホスピタルショウ2022 インタ―システムズブースのミニシアターで開催された　一般社団法人 日本IHE協会　理事　接続検証委員長　塩川 康成 様　によるご講演ビデオです。

>国際モダンホスピタルショウ　インタ―システムズブースのミニシアターでのご講演内容全般については、[InterSystems Japan YouTubeチャンネル](https://www.youtube.com/@InterSystemsJapan/playlists)にて公開しております。

{% include youtube-list.html id="_Qgv9WqrN6k" list="PLgFt3CvX3OePAiRdrL8GmMzKNiCG_BJqP" %}

> **英語ビデオもあります**
>
>- [ビデオ（英語）:What Is FHIR?](https://learning.intersystems.com/course/view.php?name=What%20is%20FHIR)
{: .block-tip}

---
## 2. <img src="./assets/icons/FHIR/Second2.png" width="70%"/>

アプリケーションのFHIR化に必要なアーキテクチャをご紹介します。

- [ビデオ（英語）:FHIR Facade Architecture Overview](https://learning.intersystems.com/course/view.php?id=2137)

    アプリケーションが HL7® FHIR® リクエストに応答できるように、FHIR ファサードアーキテクチャをセットアップする方法をご覧ください。
    
    このアーキテクチャを使用することで、InterSystems サーバーを FHIR サーバーのように扱うことができ、FHIR リポジトリを持たない環境でもFHIRリクエストをサポートできるようになります。

---
## 3. <img src="./assets/icons/FHIR/Second3.png" width="70%"/>

インターシステムズのデータ・プラットフォームで REST エンドポイントを設定し、REST を使用した FHIR 相互運用性アダプタを使用して外部の FHIR サーバとやり取りする方法を確認し、FHIR レスポンス・メッセージを入力して REST 経由で FHIR データを送信する練習をします。


- [記事：【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：（REST）APIファーストで作成するRESTディスパッチクラス](https://jp.community.intersystems.com/node/479596)

    {% include youtube-list.html id="SwquEq1fjTk" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %} 

- [記事：REST経由で情報を入力する場合の Interoperability（相互運用性機能）のサンプル](https://jp.community.intersystems.com/node/559356)　

> **英語ですが、オンラインコースもあります**
>
>- [オンラインコース（英語）:Setting Up RESTful Services](https://learning.intersystems.com/course/view.php?name=REST%20Services)
{: .block-tip}


- [ドキュメント：FHIR相互運用アダプタ](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=HXFHIR_fhir_adapter)

- [体験環境付き演習（英語）：Populating FHIR Response Messages](https://learning.intersystems.com/course/view.php?id=2272)

    FHIR ファサードとして構成された InterSystems IRIS for Health™ のインスタンスを使用して、HL7® FHIR® 要求を受け付け、InterSystems® データベースから要求されたデータを取得し、このデータを FHIR 形式で要求システムに返送するプロダクションを完成させます。

    InterSystems IRIS for Health または HealthShare® Health Connect を使用して FHIR 相互運用性ソリューションを構築する場合、FHIR 要求と応答はプロセスの不可欠な部分です。
    
    FHIR ファサードの場合、外部システムからFHIRリクエストを使用してFHIR形式のデータを要求します。データを収集し、FHIR形式に変換した後、FHIR応答メッセージをデータ要求元のシステムに送り返す必要があります。

    この演習の中では、FHIR形式に変換された患者データを受け取り、FHIR応答メッセージに情報を入力します。
    
    FHIR応答メッセージの確認方法として、REST クライアントを使用して患者データを要求し、応答メッセージが正しくFHIR形式で正しく返送されていることを確認します。

> **FHIRファサードを体験できる講師付きトレーニングコースをご提供しています**
>
> 教育サービス担当まで下記ページ末尾のお問い合わせフォームからご依頼ください。
> [問い合わせフォーム](https://www.intersystems.com/jp/course-offerings/)
{: .block-tip}

---
## 4. <img src="./assets/icons/FHIR/Second4.png" width="70%"/>

インターシステムズの標準データフォーマットであるSDAについて学び、SDAを使用して標準的なヘルスケアフォーマットのデータをFHIRフォーマットに変換する方法を学習します。

- [ドキュメント：SDAドキュメント](https://docs.intersystems.com/irisforhealthlatestj/csp/docbook/DocBook.UI.Page.cls?KEY=HXSDA_ch_sda)

- [オンラインコース（英語）:Transforming Data into the HL7 FHIR Format](https://learning.intersystems.com/course/view.php?name=FHIRTransformations)

    InterSystems IRIS for Health™ または HealthShare® Health Connect を使用して、医療システム間のデータ交換に一般的に使用されている HL7® FHIR® フォーマットにデータを変換する方法を確認できます。
    
    このコースでは、HL7 - SDA - FHIR の変換の流れを体験できます。SDA - FHIRの変換部分に、IRISのダイナミックオブジェクトを操作する方法を利用して FHIRに変換する方法を体験できます。

> **HL7 - SDA - FHIRの変換を体験できる講師付きトレーニングコースをご提供しています**
>
> 教育サービス担当まで下記ページ末尾のお問い合わせフォームからご依頼ください。
> [問い合わせフォーム](https://www.intersystems.com/jp/course-offerings/)
{: .block-tip}

- [ビデオ（英語）:Converting Legacy Data to HL7 FHIR R4 in InterSystems IRIS for Health](https://learning.intersystems.com/course/view.php?name=FHIRStarterDemo)


    このビデオでは、InterSystems IRIS® for Health のサマリー・ドキュメント・アーキテクチャ（SDA）を介して、様々なレガシーデータフォーマットを HL7® FHIR® 標準に変換する方法をご紹介します。
    
    このデモでは、InterSystems IRIS for Healthのビジネスロジックと相互運用性機能を使用して、入力されるHL7® CDA®、CSV、HL7® V2、XMLデータタイプをFHIRに変換します。
    
    このビデオで紹介するデモアプリケーションをダウンロードするには、[FHIRStarter Demo GitHub](https://github.com/intersystems/Samples-SUREFHIR)リポジトリにアクセスし、コンテナの実行手順に従ってください。また、デモを実行するにはDockerのインストールが必要です。

---
## 5. <img src="./assets/icons/FHIR/Second5.png" width="70%"/>

### FHIR JSONフォーマットを簡単に生成できるJSONTemplateエンジンについて

[JSONTemplateエンジン](https://github.com/Intersystems-jp/JSONTemplate)を利用して複雑はJSONフォーマットを簡単に生成することができます。

このテンプレートエンジンは、FHIRに限らず複雑なJSONフォーマットを生成するのに役立つエンジンです。

参考記事：[複雑なJSONの生成に便利な「JSONテンプレートエンジン」の使い方ご紹介](複雑なJSONの生成に便利な「JSONテンプレートエンジン」の使い方ご紹介)

JSONテンプレートエンジンを利用してFHIRリソースのJSONを作成する方法については以下ビデオをご参照ください。

{% include youtube-list.html id="H4LzOV-Tfzg" list="PLzSN_5VbNaxB39_H2QMMEG_EsNEFc0ASz" %}

### JSONテンプレートエンジンを利用したFHIRファサードの例

講師付きトレーニングコースで使用している[CSVからFHIRリソースを作成するFHIRファサード](https://github.com/iijimam/Training-FHIRFacadeEx)のサンプルコードを公開しています。

概要については、[README](https://github.com/iijimam/Training-FHIRFacadeEx/blob/master/readme.md)をご参照ください。


> **体験環境つき演習（英語）もあります**
>
>- [体験環境付き演習（英語）:Creating a Simple FHIR Facade](https://learning.intersystems.com/course/view.php?id=2274)
>
>    InterSystems IRIS for Health™ のインスタンスを使用して、FHIR ファサードアーキテクチャを作成および構成することで、システムが HL7® FHIR® リクエストを受け入れ、データが元々この形式で保存されていない場合でも FHIR データを返すことができます。
>
>    FHIR ファサードを作成するには、FHIR 相互運用性アダプタを使用します。
>    
>    演習の中では、特別なビジネスホストを使用してプロダクションで FHIR リクエストを処理する新しい相互運用性 REST エンドポイントを作成します。
>    
>    このプロダクションは、データの検索と変換を簡単にし、要求されたFHIR形式のデータを返送するために利用できます。
>
>    演習は、内部形式でEMRデータを保存する医療施設の FHIR ファサードを作成します。
>    この施設では、患者の詳細をJSON形式で返すREST APIが設定されていて、FHIR形式の患者データのリクエストを受けている状況です。
>
>    > HS.FHIR.DTL.vR4.Model.Resource.Patient　を使っていてダイナミックオブジェクトではない・・
{: .block-tip}



