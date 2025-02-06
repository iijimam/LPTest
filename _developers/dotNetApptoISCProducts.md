---
title: .NET アプリケーションと InterSystems 製品の接続
date: 2024-12-12
permalink: dotNetApptoISCProducts.html
layout: post
---
> オリジナルラーニングページ：[Connecting .NET Applications to InterSystems Products](https://learning.intersystems.com/course/view.php?id=968)

ADO.NET、XEP、Entity Framework、または Native API（Native SDK for .NET） を使用して、.NET アプリケーションを InterSystems IRIS® データプラットフォームやその他の　InterSystems 製品およびテクノロジに接続する方法をご説明します。

他の言語からの接続については、以下の通りです。
- [Python アプリケーションを作成する](WritingPythonAppWithInterSystems.html)

- [Java アプリケーションと InterSystems 製品の接続](JavaApptoISCProducts.html)

- [Connecting Node.js Application](https://learning.intersystems.com/course/view.php?name=Node.js%20Experience)

---
[1. <img src="./assets/icons/ServerSideApp1.png" width="40%"/>](#1-)

[2. <img src="./assets/icons/dotNet2.png" width="40%"/>](#2-)

[3. <img src="./assets/icons/dotNet3.png" width="40%"/>](#3-)

[4. <img src="./assets/icons/dotNet4.png" width="40%"/>](#4-)

[5. <img src="./assets/icons/dotNet5.png" width="40%"/>](#5-)

[6. <img src="./assets/icons/dotNet6.png" width="40%"/>](#6-)

[7. <img src="./assets/icons/dotNet7.png" width="40%"/>](#7-)

---
## 1. <img src="./assets/icons/ServerSideApp1.png" width="70%"/>

各 API の利点を確認し、.NET アプリケーションを InterSystems 製品に接続するための方法を確認します。

- ビデオ：Using .NET to Connect to InterSystems IRIS（英語／日本語字幕付き）

{% include youtube.html id="UqE7gaBHhxE" %} 

- [オンラインコース（英語）：Designing a .NET Connection Strategy](https://learning.intersystems.com/course/view.php?name=.NET%20Connection%20Strategy)


---
## 2. <img src="./assets/icons/dotNet2.png" width="70%"/>

Visual Studio プロジェクトで InterSystems ADO.NET マネージド・プロバイダを使用して、InterSystems サーバーのデータにリレーショナル・アクセスできます。

詳細は、以下ドキュメントをご参照ください。

[InterSystems IRIS デモ ： ADO.NET を使用した接続](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=AFL_adonet)

---
## 3. <img src="./assets/icons/dotNet3.png" width="70%"/>

XEP を使用して、高性能でリアルタイムのオブジェクトを迅速に格納できます。

- [ビデオ（英語／日本語字幕付き）：Using XEP with .NET](https://learning.intersystems.com/course/view.php?name=Using%20XEP%20with%20.NET)


- [ドキュメント：.NET での XEP Event Persistence の使用法](https://docs.intersystems.com/iris20241/csp/docbookj/DocBook.UI.Page.cls?KEY=BNETXEP_xep)

---
## 4. <img src="./assets/icons/dotNet4.png" width="70%"/>
Native API を使用してIRISのグローバル変数にデータを格納したり、InterSystems IRIS のメソッドまたはルーチンを呼び出します。

- [ビデオ（英語／日本語字幕付き）：Using the Native API for .NET](https://learning.intersystems.com/course/view.php?name=Native%20API%20for%20.NET)

    日本語字幕を選択できます。

- [ドキュメント：Native SDK for .NET の概要](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BNETNAT_about)

- [記事：Native SDK (NativeAPI) for .NET を使用する簡単なサンプルのご紹介](https://jp.community.intersystems.com/node/559276)

---
## 5. <img src="./assets/icons/dotNet5.png" width="70%"/>
Entity Framework Providerの使用方法を確認し、Code FirstアプローチとDatabase Firstアプローチの使用方法を学びます。

- [ドキュメント：IRISClient アセンブリの Managed Provider](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BNET_eframe)

- [ビデオ（英語／日本語字幕付き）：Using Entity Framework with InterSystems IRIS Data Platform](https://learning.intersystems.com/course/view.php?name=Entity%20Framework)


---
## 6. <img src="./assets/icons/dotNet6.png" width="70%"/>
各接続方法の利点を確認するため、体験環境を使って演習してみましょう。

[体験環境付き演習（英語）：Stock Trading with .NET](https://learning.intersystems.com/course/view.php?id=2522)

※ ビデオは日本語字幕を選択できます。

---
## 7. <img src="./assets/icons/dotNet7.png" width="70%"/>

.NET ゲートウェイを使用して、InterSystems ObjectScript で .NET オブジェクトをどのように操作できるかを確認します。

[ドキュメント：外部言語の操作](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BEXTSERV_coding)
