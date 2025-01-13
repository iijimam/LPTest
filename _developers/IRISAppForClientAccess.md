---
title: IRISを利用したWebアプリケーションの構成
date: 2024-12-09
permalink: IRISAppForClientAccess.html
layout: post
---

>オリジナル：[Configuring InterSystems IRIS Applications for Client Access](https://learning.intersystems.com/course/view.php?id=1975)

このパスでは、InterSystems IRIS® データ・プラットフォームを Web アプリケーションのバックエンドとして機能させるためのセットアップ方法をご紹介します。

具体的には、REST経由でアクセスする InterSystems IRIS アプリケーションを外部システムやユーザからデータにアクセスできるようにする方法と、JSONデータの入出力方法を簡単に行う方法を学習できます。

前提知識として、Web アプリケーションのバックエンドとして InterSystems IRIS を使用する知識を前提とし、オブジェクトと SQL の使用経験が必要です。必要に応じて、別のラーニングパス：[「InterSystems を使用してサーバーサイドアプリケーションを構築する」 ](BuidlingServerSideAppWithInterSystems.html)をご覧ください。

上記パス以外には、以下記事を利用した学習方法もあります。

- 記事： [【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その2：InterSystems IRIS で開発をはじめよう！](https://jp.community.intersystems.com/node/478601)
- 記事：[【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その3：IRIS でクラス定義を作ろう（オブジェクト操作の練習）](https://jp.community.intersystems.com/node/478606)
- [ObjectScript クックブック：ObjectScriptの基本のき！](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/Basic.md)
- 講師付きトレーニング：[InterSystems Objectのトレーニングコース（２日間）](https://www.intersystems.com/jp/intersystems-object/)

---

[1. <img src="./assets/icons/WebApp1.png" width="40%"/>](#1-)

[2. <img src="./assets/icons/WebApp2.png" width="40%"/>](#2-)

[3. <img src="./assets/icons/WebApp3.png" width="40%"/>](#3-)

---
## 1. <img src="./assets/icons/WebApp1.png" width="70%"/>
InterSystems IRIS で RESTful サービスをセットアップして、Web アプリケーションなどの外部システムからIRIS内のデータにアクセスできるようにする方法を説明します。

- [【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：IRIS で作成する REST サーバの仕組み](https://jp.community.intersystems.com/node/479546)

    IRIS で作成する RESTサーバの仕組みを解説します。

    {% include youtube-list.html id="tWP_9-jk4no" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ&index=7" %}

- [【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：（REST）手動で作成するディスパッチクラス](https://jp.community.intersystems.com/node/479551)

    RESTサーバに必要なディスパッチクラスを手動で用意する方法を解説します。

    {% include youtube-list.html id="q3XVT98_05I" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ&index=8" %}

- [【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：（REST）APIファーストで作成するRESTディスパッチクラス](https://jp.community.intersystems.com/node/479596)

    RESTサーバに必要なREST ディスパッチクラスを API ファーストの手順で作成する方法を解説します。（OpenAPI 2.0に基づいて作成したアプリケーション定義を使用してディスパッチクラスを作成する手順を解説します）

    {% include youtube-list.html id="SwquEq1fjTk" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ&index=9" %}

- [REST経由で情報を入力する場合の Interoperability（相互運用性機能）のサンプル](https://jp.community.intersystems.com/node/559356)


上記内容に関する講師付トレーニングも用意があります。

- RESTサーバの作成（1日）
- ObjectScript の使い方（1 日）


> **英語ビデオやオンラインコースもあります**
>- [体験環境付き演習:Developing REST Interfaces](https://learning.intersystems.com/course/view.php?name=DevelopingRESTInterfaces)
>
>    InterSystems IRIS® データ・プラットフォームで REST インタフェースを組み立てる方法について解説しています。
>   
>    REST は、メソッドの実行やデータのクエリのためにサーバと対話する信頼性の高い方法です。 この演習では、InterSystems IRIS サーバ、Web アプリケーション、ディスパッチ・クラスと実装クラス、および Web クライアントがどのように組み合わされて、コーヒー・メーカー会社のフロント・エンド Web サイトが作成されるかを確認していきます。
>
>- [オンラインコース：Setting Up RESTful Services](https://learning.intersystems.com/course/view.php?name=REST%20Services)
>
>   オンラインコースは IRIS の REST サーバの動作の仕組みについての解説と、体験環境付き演習内で使用しているアプリケーションの解説、REST経由で呼び出すビジネス・サービスについて学習できます。
{: .block-tip}

>《自分メモ》：フロントのWebアプリ付きの体験なら以下がいい（でも説明がない。あるけど2019のDoc）
>    リポジトリ　https://github.com/intersystems/FirstLook-REST
>
>    日本語Docだとここ　https://docs.intersystems.com/iris20191/csp/docbookj/Doc.View.cls?KEY=AFL_rest
>    （新バージョンだとないからコミュニティに手順書いて公開するのもいいかも）

---
## 2. <img src="./assets/icons/WebApp2.png" width="70%"/>

InterSystems 製品でJSONを操作するときに使用するダイナミックオブジェクト（ダイナミックエンティティ）の利用方法を学習します。

記事：[【はじめてのInterSystems IRIS】セルフラーニングビデオ：アクセス編：IRIS での JSON の操作](https://jp.community.intersystems.com/node/480106) では、以下のビデオを参照しながら、サンプルコードを試しながら進めることができるようにビデオとサンプルコードを埋め込んでいます。

ビデオだけをご覧いただく場合は、以下ご参照ください。

✅ InterSystems IRIS サーバ内でのJSONの操作

{% include youtube-list.html id="045HRug72VE" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ&index=10" %}

✅ JSONの操作　つづき：SQL関数と%JSON.Adapterを使ってみる
    {% include youtube-list.html id="3YKkFqJj2G8" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ&index=11" %}

✅ JSONの操作　つづき：ダイナミックエンティティのメソッドを使ってみる
    {% include youtube-list.html id="4ZIsetgJaxA" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ&index=12" %}


> **英語ビデオやオンラインコースもあります**
>- [オンラインコース：Using JSON in InterSystems IRIS](https://learning.intersystems.com/course/view.php?name=JSON%20in%20IRIS)
>
>   ダイナミックオブジェクトを使用して JSON をモデル化し、InterSystems IRIS® データプラットフォームで、JSON データを扱う方法を学習します。
>
>   また、JSONデータの取得と生成、エラーの処理、およびアプリケーションのトラブルシューティングの方法について説明します。
>
>   最後に、レストランの利用者がレストランを評価し、その評価をGoogle Placesから取得した既存のレビューに追加するアプリケーションを構築します。このシナリオの詳細については、コースの最初のセクションを参照してください。
{: .block-tip}



## 3. <img src="./assets/icons/WebApp3.png" width="70%"/>

InterSystems API Manager の紹介と、InterSystems IRIS アプリケーションで使用する API へのトラフィックの監視と制御方法を確認します。

- [ゼロから使いこなす IAM（InterSystems API Manager）](https://jp.community.intersystems.com/node/493416)

> **英語ビデオもあります**
>
>- [ビデオ：What is InterSystems API Manager](https://www.youtube.com/watch?v=XI1oqKEwLL0)
{: .block-tip}

