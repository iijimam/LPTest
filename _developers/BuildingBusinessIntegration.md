---
title: ビジネス・インテグレーションの構築
date: 2024-12-08
permalink: BuildingBusinessIntegration.html
layout: post
---

>オリジナル[Building Business Integrations with InterSystems IRIS](https://learning.intersystems.com/course/view.php?id=1437)

InterSystems 製品の相互運用性（Interoperability）フレームワークによりインターフェイスエンジニアやソフトウェア開発者は、複数のシステムを接続し下流のアプリケーションにメッセージを迅速にルーティングすることができます。

このパスでは、統合（インテグレーション）の基本を学び組み込みオプションやカスタムオプションを使用してデータを送信、受信、処理、変換する方法を確認できます。

[1. <img src="./assets/icons/1.png" width="40%"/>](#1-)

[2. <img src="./assets/icons/BIntegration2.png" width="40%"/>](#2-)

[3. <img src="./assets/icons/BIntegration3.png" width="40%"/>](#3-)

---
## 1. <img src="./assets/icons/1.png" width="70%"/>

最初に、IRISのInteroperability（相互運用性）機能でどのようなことができ、どのような開発が必要になるかについて確認します。

- ビデオ：Interoperability概要

    12分以降をご覧ください。

    {% include youtube-list.html id="vo12UnH-c-s" list="PLzSN_5VbNaxD-r8wU4LHwLwGSzUjrffEX&index=1&t=1203s" %}

- シリーズ記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：動作の仕組みを知ろう](https://jp.community.intersystems.com/node/483036)

- シリーズ記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：プロダクションとは](https://jp.community.intersystems.com/node/483041)


> **英語ビデオやオンラインコースもあります**
>
> - [体験環境付き演習：Receiving and Routing Data in a Production](https://learning.intersystems.com/course/view.php?name=Interop%20QS)
>
>   - 演習概要はこちら（Interoperability QuickStart）👉　https://www.intersystems.com/jp/quickstart/
>
>   - 演習内容👉http://github.com/intersystems/Samples-Integration-RedLights
>
>- [オンラインコース（英語）:Integration Architecture](https://learning.intersystems.com/course/view.php?id=908)
>
>    InterSystems IRIS®データプラットフォーム、InterSystems HealthShare®、InterSystems Ensemble® の統合機能の基本的なアーキテクチャを学習します。これらのコンポーネントを通じてデータがどのように流れ、システム間の相互運用が可能になるかを学びます。
>
>    このコースには、3 つのレッスンと数問のクイズが含まれています。ビデオはフルスクリーンモードでご覧ください。
{: .block-tip}

---
## 2. <img src="./assets/icons/BIntegration2.png" width="70%"/>
InterSystems IRIS に組み込まれているグラフィカル・ツールを使用して、メッセージを取り込み、正しい形式で下流のシステムに渡します。

- 記事：[レコードマップで何ができるか？](https://jp.community.intersystems.com/node/494326)

- 記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・オペレーション）](https://jp.community.intersystems.com/node/483136)  


> **英語ビデオやオンラインコースもあります**
>- [ビデオ（英語）：Record Mapper Introduction](https://learning.intersystems.com/enrol/index.php?id=1094)
>
>- [オンラインコース（英語）:Building BPL Business Processes](https://learning.intersystems.com/course/view.php?name=Building%20BPL%20Business%20Processes)
>
>    管理ポータルのビジネス・プロセス・デザイナーを使用して、BPLビジネス・プロセスを構築する方法を学びます。このコースには、6つのインストラクションレッスンといくつかのクイズ問題が含まれています。ビデオはフルスクリーンモードで見るのが最適です。
>
>    このオンラインコース受講に必要な前提知識は以下の通りです。（コンポーネントそれぞれの役割とプロダクション構成の画面操作ができること＋ビジネスオペレーションの作成方法を知っていること）
>
>    - [Integration Architecture](https://learning.intersystems.com/course/view.php?name=Integration%20Architecture)
>
>    - [オンラインコース（英語）:Building Custom Business Operations](https://learning.intersystems.com/course/view.php?name=Building%20Custom%20Business%20Operations)
>
>    - [ビデオ（英語）:Setting Up Business Rules](https://learning.intersystems.com/course/view.php?id=1295)
>
>    - [オンラインコース（英語）:Data Transformations Basics](https://learning.intersystems.com/enrol/index.php?id=1170)
>
>        グラフィカルな管理ポータル・インタフェースを使用して、データ変換を作成する方法を学びます。フィールドをマップする方法、フィールドを変更する関数を使用する方法、およびフィールドの値としてリテラルを使用する方法をご覧ください。最後に、変換をテストして実装する方法を学びます。
>
>   >メモ：前提知識にHL7について知っていることが含まれています。
{: .block-tip}

---
## 3. <img src="./assets/icons/BIntegration3.png" width="70%"/>

プロダクションですぐに使える機能をの他に、ニーズに合わせて ObjectScript を使用してカスタムコンポーネントを作成することができます。

- 記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：メッセージ](https://jp.community.intersystems.com/node/483131)

- 記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・オペレーション）](https://jp.community.intersystems.com/node/483136)
- 記事：[【はじめてのInterSystems IRIS】Interoperability（相互運用性）：コンポーネントの作成（ビジネス・サービス）](https://jp.community.intersystems.com/node/483186)

    - 記事：[REST経由で情報を入力する場合の Interoperability（相互運用性機能）のサンプル](https://jp.community.intersystems.com/node/559356)

> **英語ビデオやオンラインコースもあります**
- [ビデオ（英語）：Building Custom Production Messages](https://learning.intersystems.com/course/view.php?name=Custom%20Messages)
>
>- [オンラインコース（英語）：Building Custom Business Operations](https://learning.intersystems.com/course/view.php?name=Building%20Custom%20Business%20Operations)
>
>- [オンラインコース（英語）:Building Custom Business Services (1h 30m)](https://learning.intersystems.com/enrol/index.php?id=2031)
{: .block-tip}

