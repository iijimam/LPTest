---
title: Python アプリケーションを作成する
date: 2024-12-10
permalink: WritingPythonAppWithInterSystems.html
layout: post
---
> オリジナル：[Writing Python Applications with InterSystems](https://learning.intersystems.com/course/view.php?id=1943)

既存の Python コーディングスキルを活用して、InterSystems® アプリケーションを強化します。

このパスでは、クライアントの Python アプリケーションから InterSystems サーバーに接続する方法、InterSystems ObjectScript コードに Python を組み込む方法（Embedded Python）、Python ライブラリの呼び出しに負荷のかかる処理が必要な場合に別のサーバーある InterSystems サーバーを呼び出す方法について学習します。

なお、このパスは、Pythonの基本的なコーディング経験があることを前提としています。必要に応じて、[Python for Beginners](https://www.python.org/about/gettingstarted/)をご覧ください。

---
[1. <img src="./assets/icons/1.png" width="40%"/>](#1-)

[2. <img src="./assets/icons/Python2.png" width="40%"/>](#2-)

[3. <img src="./assets/icons/Python3.png" width="40%"/>](#3-)

[4. <img src="./assets/icons/Python4.png" width="40%"/>](#4-)

---
## 1. <img src="./assets/icons/1.png" width="70%"/>

InterSystems のアプリケーションで Python ライブラリを活用する方法をご説明します。

pyodbc を使用して既存の Python アプリケーションを接続したり、Embedded Python（または「組み込み Python」） を使用して、Python プログラムを ObjectScrit で記述されたプログラムと同等の位置付けで実行できます。

また、InterSystems Native API または外部言語サーバを使用して、Python で完全な InterSystems アプリケーションを構築することもできます。

![](./assets/icons/PythonLP-1.png)

Python 開発者が、InterSystems 製品を使用してアプリケーションを構築する場合、いくつかのオプションを選択できます。

- **pyodbc** を使用する方法

    従来のクライアント・サーバーアーキテクチャで ODBC を使用して既存の Python アプリケーションとInterSystems サーバを接続します。

    Pyodbc は DB API 2.0 仕様を実装しています。ODBC を使用して SQL クエリを作成し、データを取得します。

- **Embedded Python** を使用する方法

    Python プログラムを ObjectScrit で記述されたプログラムと同等の位置付けで実行できます。

- その他の方法

    - **InterSystems Python Native API** を使用して、InterSystems IRIS クラスおよびグローバルを操作できます。

    - **外部言語サーバー**を使用して、InterSystems IRIS カーネルの外部で Python コードを実行できます。
    
        外部言語サーバは、プロセス外または InterSystems IRIS とは別のサーバで実行する必要がある Python アプリケーションに適用できます。
        
        例えば、CPU やメモリの使用率が高い場合や、コードの安定性に疑問がある場合に使用します。

---
## 2. <img src="./assets/icons/Python2.png" width="70%"/>

Python アプリケーションを　InterSystems 製品に接続するための最も一般的なオプションである pyodbc の使用方法について説明します。

- [ドキュメント:pyodbc Python ODBC ブリッジのサポート](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BNETODBC_support_pyodbc)


- [【はじめての InterSystems IRIS】セルフラーニングビデオ：アクセス編：Python から PyODBC を使って IRIS に接続してみよう](https://jp.community.intersystems.com/node/478616)

{% include youtube-list.html id="_Qgv9WqrN6k" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ&index=6" %}

---
## 3. <img src="./assets/icons/Python3.png" width="70%"/>

Embedded Python を使用して、ObjectScript と並行して Python ライブラリを呼び出すことができます。

{% include youtube.html id="qhNnS7rN7XE" %} 
上記ビデオの日本語字幕入りビデオ👉[What Is Embedded Python?](https://learning.intersystems.com/course/view.php?name=EmbeddedPythonOverview)

- [ビデオ（英語／日本語字幕あり）：演習環境付き演習：Embedded Python QuickStart](https://learning.intersystems.com/course/view.php?name=EmbeddedPythonQS)

> **英語ですが、オンラインコースもあります**
>- [Parsing Images and Charting Data with Embedded Python](https://learning.intersystems.com/course/view.php?id=2126)
{: .block-tip}

↑上記オンラインコース演習と同等の内容をお試しいただける記事👉[Embedded Python を使ってレシート（JPG）の中身を IRIS に登録してみました](https://jp.community.intersystems.com/node/513136)

---
**【オプションビデオ：Embedded Python のセルフラーニングビデオのプレイリスト】**

✅ [IRISでPythonを使ってみよう](https://www.youtube.com/playlist?list=PLzSN_5VbNaxBLXlC9oCgwPtxBilT8tJ96)-PythonスクリプトファイルをObjectScriptを使用して呼び出す（IRIS ターミナルからPythonスクリプトファイルに記載した内容を呼び出す）

{% include youtube-list.html id="awiRCQnm5Vo" list="PLzSN_5VbNaxBLXlC9oCgwPtxBilT8tJ96&index=6" %} 

✅ [IRISでPythonを使ってみよう](https://www.youtube.com/playlist?list=PLzSN_5VbNaxBLXlC9oCgwPtxBilT8tJ96)-Pythonの組み込み関数をObjectScriptで使用する方法

{% include youtube-list.html id="dyx4wNw51YU" list="PLzSN_5VbNaxBLXlC9oCgwPtxBilT8tJ96&index=9" %} 

✅ [IRISでPythonを使ってみよう](https://www.youtube.com/playlist?list=PLzSN_5VbNaxBLXlC9oCgwPtxBilT8tJ96)-参考情報：グローバル変数の操作

{% include youtube-list.html id="XzWeCICH0VY" list="PLzSN_5VbNaxBLXlC9oCgwPtxBilT8tJ96&index=18" %}

✅ [SQLアクセス編](https://www.youtube.com/playlist?list=PLzSN_5VbNaxDAPjSBe5F-uGbGkoJqcerL)-Sample.Personの作成（実演）- Pythonシェルで Embedded Python を利用して IRIS にあるテーブルにアクセスする

{% include youtube-list.html id="hJs3JUzWoWE" list="PLzSN_5VbNaxDAPjSBe5F-uGbGkoJqcerL&index=5" %}

✅ [オブジェクトアクセス編](https://www.youtube.com/playlist?list=PLzSN_5VbNaxBnEb5rq-676b1l7Ym6INjL)-インスタンス生成から保存までの実演

{% include youtube-list.html id="Ayir9SgMId8" list="PLzSN_5VbNaxBnEb5rq-676b1l7Ym6INjL&index=7" %}

> **英語オプションビデオもあります**
>
>- [Using Python Libraries from ObjectScript with Embedded Python](https://learning.intersystems.com/course/view.php?name=PythonLibrariesOS)
>
>    このビデオでは、IRIS ターミナルを利用して ObjectScript から Python を実行する方法を解説しています。
>
>- [Leveraging Embedded Python in Interoperability Productions](https://learning.intersystems.com/course/view.php?name=Embedded%20Python%20with%20Interoperability)
>
>    InterSystems サーバーの Interoperability プロダクションで Embedded Python を活用する方法を解説しています。
>    
>    ビジネスホストのコンテキストとライフサイクルにおける Embedded Python の利点について学習できます。また、AWS SNS と OPC UA サーバとの統合デモをご覧いただき、Embedded Python を使ったビジネスホストの構築方法をご紹介します。
>
>- [Using the InterSystems IRIS Library from Embedded Python](https://learning.intersystems.com/course/view.php?name=Embedded%20Python%20for%20ObjectScript%20Developers:%20Working%20with%20Python%20and%20ObjectScript%20Side-By-Side)
>
>    Python を使用して InterSystems IRIS® データプラットフォームと対話する方法をご紹介します。
>    
>    Embedded Python を使用すると、InterSystems ObjectScript と Python を同時に使用できます。
>   このビデオでは、Pyhtonシェルの中から IRIS のクラスのインスタンスを生成したり、メソッドを実行する例、またグローバル変数の操作例、SQLの実行例をご覧いただけます。
{: .block-tip}

- [ドキュメント：組み込み Python の概要](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=AFL_epython)

- [ドキュメント：組み込みPythonの使用法](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GEPYTHON)

---
## 4. <img src="./assets/icons/Python4.png" width="70%"/>

InterSystems Python SDK を使用して、Python から InterSystems IRIS クラスのインスタンスをリモートで作成および操作できます。また、外部言語サーバを使用して、InterSystems 製品から外部プロセスで実行されている Python コードを呼び出す方法をご紹介しています。


✅[【はじめての InterSystems IRIS】セルフラーニングビデオ：アクセス編：Python の NativeAPI に挑戦](https://jp.community.intersystems.com/node/478611)

{% include youtube-list.html id="esRyiWaIofg" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ&index=5" %}


> **英語ですが、オンラインコースもあります**
>
>- [ビデオ（英語）:Using the Native API for Python](https://learning.intersystems.com/enrol/index.php?id=1110)
>
>- [演習環境付き演習（英語／ビデオに日本語字幕あり）:Python QuickStart](https://learning.intersystems.com/enrol/index.php?id=1113)
>
>    InterSystems IRIS® データ・プラットフォームは、リレーショナル・テーブルまたは多次元ストレージを介した InterSystems IRIS データベースへの直接アクセスを提供する 2 つの軽量な Python API をサポートしています：
>
>    - PyODBC を使用すると、アプリケーションはデータを迅速に取得、更新、削除できます。
>    - Python Native API を使用すると、アプリケーションは、ObjectScript のメソッドやルーチンを呼び出すだけでなく、InterSystems IRIS 内の基礎となるデータ構造 (グローバルとして知られている) に直接アクセスできます。
>    
>    ビデオでアプリケーションを InterSystems IRIS に接続する方法を確認し、以下の演習で PyODBC と Native API for Python を使用して InterSystems IRIS に接続してみてください。
>
>- [体験環境付き演習（英語／ビデオに日本語字幕あり）Interacting with Data in Python Using Multiple Data Models](https://learning.intersystems.com/course/view.php?name=PythonMultiModel)
>    
>    InterSystems IRIS® データ・プラットフォームのマルチモデル・アーキテクチャをお試しください。
>
>   InterSystems IRIS のマルチ・モデル・アクセスは、グローバルと呼ばれるデータ構造によって実現されています。これにより、データの重複を回避しながら、柔軟なデータ・アクセスが可能になります。
>
>    Python では、Native API を使用して InterSystems IRIS に接続し、グローバルを使用してデータを操作できます。もう 1 つのオプションは、PyODBC で接続し、業界標準の SQL を使用してデータにアクセスする方法です。この場合、データはリレーショナル・テーブルとしてモデル化されます。
{: .block-tip}

- [ドキュメント：外部言語の操作](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=BEXTSERV_coding)

