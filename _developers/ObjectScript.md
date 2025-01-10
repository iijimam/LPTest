---
title: InterSystems ObjectScript入門
date: 2024-12-06
permalink: ObjectScript.html
layout: post
---

>オリジナル：[Getting Started with InterSystems ObjectScript](https://learning.intersystems.com/course/view.php?id=289)

InterSystems ObjectScript の基本的な構文と主要な要素について学習します。

[1. <img src="./assets/icons/O1.png" width="40%"/>](#1-)

[2. <img src="./assets/icons/O2.png" width="40%"/>](#2-)

[3. <img src="./assets/icons/O3.png" width="40%"/>](#3-)

[4. <img src="./assets/icons/O4.png" width="40%"/>](#4-)

---
## 1. <img src="./assets/icons/O1.png" width="70%"/>

ObjectScript 概要、変数、式、コマンドなど、主な機能のいくつかを学習します。

- [ドキュメント：ObjectScriptの概要](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCOS_intro)

- [ObjectScriptクックブック：ObjectScriptの基本のき！](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/Basic.md)

    実際のコマンド操作を試す場合にはIRISのインストール環境、または、オンラインコース（英語）の利用が必要です。
    
    IRISのインストール方法については、以下ビデオをご参照ください。
    
    {% include youtube-list.html id="nKDvM68Gs04" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %}

> **英語ビデオやオンラインコースもあります**
>
>- [オンラインコース：InterSystems ObjectScript Basics（英語）](https://learning.intersystems.com/course/view.php?name=Cach%C3%A9%20ObjectScript%20Basics)
>
>    オンラインコースを通して以下の内容を学習できます。
>    - InterSystems ObjectScript における変数の型付け方法
>    - 変数の型に関する詳細情報をドキュメントから検索する方法
>    - 変数の設定、変数の内容の確認、および変数のメモリからの削除を行うための set、write、kill の使用方法
>    - 算術演算と組み込み関数を使用して変数を操作する
>    - 論理演算子を使用して変数を比較する
>    - if/else 文を評価する。
>    - do を使ってメソッドを実行する
>    - ループを使用する
{: .block-tip}


---
## 2. <img src="./assets/icons/O2.png" width="70%"/>

演算子と式の記述方法を確認します。また、ObjectScriptが提供する関数の利用方法も学習します。

最後に、コマンドの後置条件式の記述方法を確認します。

- [ドキュメント：演算子と式](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCOS_operators)

- [ObjectScriptクックブック：演算子](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#%E6%BC%94%E7%AE%97%E5%AD%90)

- 関数操作：[ObjectScriptクックブック：文字列操作](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#%E6%96%87%E5%AD%97%E5%88%97%E6%93%8D%E4%BD%9C)

    文字列の操作に便利な関数の説明が含まれています。

> **関数について、英語ビデオもあります**
>
>- ビデオ（英語）：Using System Functions in ObjectScript
{: .block-tip}
{% include youtube-list.html id="Mx3WNXMPxpiE" list="PLp4xNHWZ7IQmiSsryS0T3qjuVXlbSWqc8&index=4" %}


- ビデオ（英語）：Controlling Command Flow with Postconditional Expressions
   
   If 文を使用せずに単一のコマンドに条件を追加する方法（後置条件）を説明しています。
   
   InterSystems ObjectScript では、ほとんどの単一行コマンドの後ろに後置条件を追加することで、コマンド・フローを制御できます。後置条件は、コマンドが実行されるべきかどうかを決定します。

    {% include youtube-list.html id="4RgA213AhF8" list="PLp4xNHWZ7IQmiSsryS0T3qjuVXlbSWqc8" %}



---
## 3. <img src="./assets/icons/O3.png" width="70%"/>

ObjectScript の変数の特徴を理解します。またObjectScriptが提供する特殊変数とその使用方法についても学習します。

- 変数について

    ✅ [ObjectScriptの基本のき！：変数](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/Basic.md#3-%E5%A4%89%E6%95%B0%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6)

    ✅ [注意点](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#%E6%B3%A8%E6%84%8F%E7%82%B9)

    ✅ [ドキュメント：多次元配列](https://docs.intersystems.com/irislatest/csp/docbook/DocBook.UI.Page.cls?KEY=GCOS_mdarrays)

    ✅ 特殊変数：[現在日付と時刻の取得](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#%E7%8F%BE%E5%9C%A8%E6%97%A5%E4%BB%98%E3%81%A8%E6%99%82%E5%88%BB%E3%81%AE%E5%8F%96%E5%BE%97)


- [リスト操作方法](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#%E3%83%AA%E3%82%B9%E3%83%88)

- インスタンス操作方法

    IRISに作成したクラス定義のインスタンス操作について説明しているビデオをご覧ください。（例では永続のタイプのクラスを定義し、インスタンスを生成しプロパティに値を代入した後、データベースに値を保存する流れを確認できます。）

    > 27:40からインスタンス生成の説明が登場します。

    {% include youtube-list.html id="kWJCzn9bndQ" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %}

> **英語ビデオもあります**
>
>- ビデオ（英語）：Exploring Data Types in ObjectScrip
{: .block-tip}
{% include youtube-list.html id="MSWccht-eGI" list="PLp4xNHWZ7IQmiSsryS0T3qjuVXlbSWqc8&index=2" %}

>
>- ビデオ（英語）：Using Variables in ObjectScript
{: .block-tip}
{% include youtube-list.html id="FCYi0Y0xeTw" list="PLp4xNHWZ7IQmiSsryS0T3qjuVXlbSWqc8" %}


---
## 4. <img src="./assets/icons/O4.png" width="70%"/>
ObjectScript の基本を学習できましたので、Visual Studio Code を利用してクラス定義を作成します。

以下のビデオでは、クラス定義の作成からインスタンス生成、保存までの流れを確認できます。

{% include youtube-list.html id="kWJCzn9bndQ" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %}

> **英語のオンラインコースもあります**
>
>- [オンラインコース（英語）:Creating an InterSystems Class Definition in VS Code](https://learning.intersystems.com/course/view.php?name=IRIS%20Class)
{: .block-tip}

VSCode用ラーニングパスもあります。[VS Codeを使用したInterSystemsサーバサイドの開発](/VSCode.html)をご参照ください。
