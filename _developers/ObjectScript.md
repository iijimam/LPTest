---
title: InterSystems ObjectScript 入門
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

ObjectScript 概要、変数、式、コマンドなど主な機能のいくつかを学習します。

- <a href="https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCOS_intro" target="_blank">ドキュメント：ObjectScriptの概要</a>

- <a href="https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/Basic.md" target="_blank">ObjectScriptクックブック：ObjectScriptの基本のき！</a>

    実際のコマンド操作を試す場合には IRIS のインストール環境、または、オンラインコース（英語）の利用が必要です。
    
    IRISのインストール方法については、以下ビデオをご参照ください。
    
    {% include youtube-list.html id="nKDvM68Gs04" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %}

<br>
> **英語ビデオやオンラインコースもあります**
>
>- <a href="https://learning.intersystems.com/course/view.php?name=Cach%C3%A9%20ObjectScript%20Basics" target="_blank">オンラインコース：InterSystems ObjectScript Basics（英語）</a>
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

演算子と式の記述方法を確認します。また、ObjectScript が提供する関数の利用方法も学習します。

最後に、コマンドの後置条件式の記述方法を確認します。

- <a href="https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCOS_operators" target="_blank">ドキュメント：演算子と式</a>

- <a href="https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#%E6%BC%94%E7%AE%97%E5%AD%90" target="_blank">ObjectScriptクックブック：演算子</a>

- 関数操作：<a href="https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#%E6%96%87%E5%AD%97%E5%88%97%E6%93%8D%E4%BD%9C" target="_blank">ObjectScriptクックブック：文字列操作</a>

    文字列の操作に便利な関数の説明が含まれています。

> **関数について、英語ビデオもあります**
>
>- ビデオ（英語）：Using System Functions in ObjectScript
{: .block-tip}
{% include youtube-list.html id="Mx3WNXMPxpiE" list="PLp4xNHWZ7IQmiSsryS0T3qjuVXlbSWqc8&index=4" %}

<details class="transcript2">
<summary> ▶日本語字幕 </summary>
<div class="content">
InterSystems ObjectScript には、コマンドラインで呼び出すことができる組み込みのシステム関数が多数用意されておりデータを簡単に扱うことができます。ObjectScript のシステム関数 ($Length() など) は、$ 記号のプレフィックスで始まります。
<br>
関数は、受け取った引数に対してさまざまな処理を実行します。操作には、文字列の操作、リストまたはビット文字列の作成、クラスメソッドの実行、値の検証などがあります。
<br>
関数名の後に括弧で引数を指定します。そして関数は操作の結果である値を返します。
<br>
ほとんどの場合、関数の戻り値はコマンドや別の関数に渡されます。よくある例は、関数の戻り値を write コマンドの引数として与えることです。
<br>
これを実際に見るために $Length() 関数を詳しく見てみましょう。この関数の必須引数はひとつで対象となる文字列を表す式です。引数は、使用する関数によって異なります。
<br>
試しに、括弧内に 「How long is this string?」 という引数を指定して $Length 関数を実行し、この関数が返す値を write コマンドに与えてみましょう。write $Length(「この文字列の長さは？」)を実行すると文字列の長さが 24 文字であることがわかります。
<br>
また、関数は 1 つ以上の引数を取ることができるということも重要です。この例では、文字列 「How long is this string?」 が $Length 関数に必要な唯一の引数です。しかし、他の関数では複数の引数を取ることがありその場合はカンマで区切らなければなりません。
<br>
例えば $Piece() 関数は、区切り文字の有無で部分文字列を識別します。文字列の最初の単語を取得したい場合、この関数には 3 つの引数が必要です。write $Piece() というコマンドを実行し、3つの引数を与えてみよう。文字列、デリミタ（この場合はスペース）、そして取り出す部分文字列の位置 1 を指定します。
<br>
部分文字列が返されると、それが write コマンドに渡され最初の単語が抽出されていることを確認できます。
<br>
関数の戻り値を別の関数で使うこともできます。例えば、今取り出した単語の長さを知りたいとします。
<br>
この結果を得るには、先ほど実行した $Piece() 関数を $Length() の引数として与えその結果を write します。
<br>
これは、文字列の最初の単語の長さが 3 文字であることを示します。
<br>
$Piece() 関数は部分文字列の置換にも使えます。これまで実行した関数は引数を変更しませんでしたが、set コマンドで実行すると引数を変更できる関数もあります。
<br>
まず次の変数をセットしてみよう： sentence = 「How long is this string?」。次に、次のコマンドを実行します。 set $Piece( = 「Video」. Pieceの3つの引数は、文字列を保持する変数である sentence、区切り文字、置換したい部分文字列の位置を指定します。次に、変数: sentence を write します。これは、文の5番目の部分文字列 string を引数に指定した文字列 video に置き換えるものである。
<br>
システム関数には、$Piece() のように 2 種類の使い方ができるものがたくさんある。その使い方によって関数が引数を変更するかどうかが決まります。
<br>
これまで、文字列関数の例を見てきました。ObjectScript の他の種類の関数を使用するとより複雑な変数の構築などのアクションを実行できます。
<br>
たとえば、$ListBuild() 関数は、指定された項目で構成されるリスト変数を作成するために使用します。注文の詳細を保持するためにいくつかの変数を設定してみましょう。OrderDate=「2022年6月15日」、Amount=25、Status=「処理中 」とします。これらの変数を設定したので、$ListBuild() 関数の引数として与えて 3 つすべてを含むリスト変数を作成することができます。
<br>
この場合、set コマンドを使用して、$ListBuild() 関数の返り値に等しい変数を設定します。リスト変数を作成するには set Order = $ListBuild(OrderDate, Amount, Status) を実行します。
<br>
次に、Order を記述してリストが正常に構築されたことを確認します。リスト変数を書き込むには、zwrite コマンドを使用します。
<br>
リストには、設定した 3 つの項目、すなわち注文日、金額、ステータスが含まれていることがわかります。リスト変数の項目を更新するには、$List() 関数を使います。ステータスを 「Complete 」に変更して、もう一度 zwrite Order を実行してみましょう。
<br>
これで、ObjectScript でシステム関数を適切にフォーマットして実行する方法がわかったと思います。
</div>
</details>

<br>
- ビデオ（英語）：Controlling Command Flow with Postconditional Expressions
   
   If 文を使用せずに単一のコマンドに条件を追加する方法（後置条件）を説明しています。
   
   InterSystems ObjectScript では、ほとんどの単一行コマンドの後ろに後置条件を追加することで、コマンド・フローを制御できます。後置条件は、コマンドが実行されるべきかどうかを決定します。

    {% include youtube-list.html id="4RgA213AhF8" list="PLp4xNHWZ7IQmiSsryS0T3qjuVXlbSWqc8" %}

<details class="transcript2">
<summary> ▶日本語字幕 </summary>
<div class="content">
InterSystems ObjectScript プログラマとして、コマンド・フローを制御するためのいくつかのオプションがあります。一般的には if 文を使用しますが、特に 1 行のコードを記述する場合など、条件が真であるときに 1 つのコマンドを実行するための迅速な方法が必要な場合があります。
<br>
if 文を書く代わりに実行すべきかどうかを示す後置条件式をコマンドに付加することができます。
<br>
これは do や execute コマンドの引数にも有効です。
<br>
このビデオの例はすべてコマンドに言及していますが、同じ構文はコマンド引数にも当てはまります。構文は簡単です。コマンド・キーワード（この例では write）を入力しその後にコロンを続けます。コロンでコマンドと後置条件を区切り、コロンの両側にはスペースを入れません。
<br>
コロンの直後には、コマンドが実行されるかどうかを決定する後置条件を置きます。構文エラーを避けるために条件を括弧で囲むのがベストプラクティスです。
<br>
括弧で囲まれていない限り、空白は許可されません。条件に続くのは引数で、条件が真の場合に実行されます。式が真になるとはどういうことかを少し確認してみましょう。
<br>
このコードでは、変数 a が変数 n 以下であるという条件が真であれば、write コマンドで「バナナが大好きです」という文を出力します。
<br>
条件が複雑であったりスペースが必要な場合は、括弧で囲みます。たとえば、2 つの条件をそれぞれ括弧で囲み、and 演算子（2つの&）で結合します。条件全体を括弧で囲むことで、両方の条件を考慮する必要があることを示します。
<br>
InterSystems Terminal の簡単な例を確認してみましょう。変数 a は現在 3、で変数 b は 0 です。
<br>
a の値が 5 より大きい場合に b の値を変更したいとします。これを行うには、set コマンドにコロンをセパレーターとして使用した後置条件を追加します。a が 5 より大きければ、b は 10 になる。
<br>
コマンドを入力すると、b の値はゼロになる。なぜなら、a は以前に 3 に設定されていたからである。
<br>
では、条件を満たすように変数 a を 6 に設定してみよう。再び set コマンドを実行するととなり、変数 b の値は 10 に設定されます。
<br>
ObjectScript の条件は、結果が有効なゼロ以外の数値であれば真になります。
<br>
この動作を確認するために、3 つの変数を設定してみましょう。数値変数 a に 12 を設定し、次に b に値 12 の文字列を設定します。また、文字列変数 c に値 「40 musicians」を設定します。
<br>
write コマンドを入力すると、条件変数 a に対して値 「True 」が返されます。
<br>
変数 b と c についても同様です。
<br>
c は musicians という単語を含んでいるにもかかわらず、40 というゼロでない数字で始まっています。そのため、ObjectScript はこれを真と評価します。
<br>
a に 0、bに値 0 の文字列、c に 「The 40 musicians 」を設定したらどうなるでしょうか。同じコマンドを入力すると
<br>
a と b は 0 なので、条件はすべて偽で、c は単語で始まるので、ObjectScript はこれを値 0 として認識します。
<br>
後置条件式は、変数が数値であれ文字列であれ条件がゼロでない場合にのみコマンドを実行します。
<br>
後置条件式は、2 つのタイプを除いてあらゆる ObjectScript コマンドで使用できます。
<br>
まず、IF、ELSEIF、ELSE、FOR、WHILE、DO WHILE などのフロー制御コマンドでは使用できません。というのも、後置条件もコマンド・フローを制御するのでコード内で両方を使うと冗長になるからです。
<br>
これらを一緒に使おうとすると、システムは構文エラーを表示します。
<br>
次に、TRY や CATCH のようなエラー処理コマンドと一緒に後置条件を使うことはできません。
<br>
同じ条件で複数のコマンド行を作成する必要がある場合は、他の開発者がコードを読みやすくするために if 文を使用するのが最善です。各コマンドの後に同じ後置条件を書く代わりに、if 文の後に中括弧でコマンドのリストを書きます。
<br>
1 つのコマンドラインに条件を書く場合、後置条件式は使いやすいオプションです。
<br>
後置条件とコマンドの詳細については、ドキュメントをご覧ください。
</div>
</details>
<br>
---
## 3. <img src="./assets/icons/O3.png" width="70%"/>

ObjectScript の変数の特徴を理解します。また ObjectScript が提供する特殊変数とその使用方法についても学習します。

- 変数について

    ✅ <a href="https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/Basic.md#3-%E5%A4%89%E6%95%B0%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6" target="_blank">ObjectScriptの基本のき！：変数</a>

    ✅ <a href="https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#%E6%B3%A8%E6%84%8F%E7%82%B9" target="_blank">注意点</a>

    ✅ <a href="https://docs.intersystems.com/irislatest/csp/docbook/DocBook.UI.Page.cls?KEY=GCOS_mdarrays" target="_blank">ドキュメント：多次元配列</a>

    ✅ 特殊変数：<a href="https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#%E7%8F%BE%E5%9C%A8%E6%97%A5%E4%BB%98%E3%81%A8%E6%99%82%E5%88%BB%E3%81%AE%E5%8F%96%E5%BE%97" target="_blank">現在日付と時刻の取得</a>


- <a href="https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#%E3%83%AA%E3%82%B9%E3%83%88" target="_blank">リスト操作方法</a>

- インスタンス操作方法

    IRISに作成したクラス定義のインスタンス操作について説明しているビデオをご覧ください（例では永続のタイプのクラスを定義し、インスタンスを生成しプロパティに値を代入した後、データベースに値を保存する流れを確認できます）。

    > 27:40からインスタンス生成の説明が登場します。

    {% include youtube-list.html id="kWJCzn9bndQ" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %}

<br>
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
<br>
> **英語のオンラインコースもあります**
>
>- <a href="https://learning.intersystems.com/course/view.php?name=IRIS%20Class" target="_blank">オンラインコース（英語）:Creating an InterSystems Class Definition in VS Code</a>
{: .block-tip}

VSCode用ラーニングパスもあります。<a href="VSCode.html" target="_blank">VS Codeを使用した InterSystems サーバサイドの開発</a>をご参照ください。
