---
title: HL7 FHIRとは
date: 2024-12-01
permalink: IntroFHIRStandard.html
layout: post
---

> オリジナルページ：[Introduction to the FHIR Standard](https://learning.intersystems.com/course/view.php?id=2401)

HL7® FHIR® を世界をリードするヘルスケアデータ標準にしている多くの特徴と機能について学びます。

このラーニング・パスでは、FHIR 標準がどのように機能し、最新のヘルスケアアプリケーションでどのように使用されるかをビデオを利用して学習します。

最後に、FHIR データモデルの実習を行った後、FHIRについてよくある質問についてもお答えします。


[1. <img src="./assets/icons/FHIR/Intro1.png" width="40%"/>](#1-)

[2. <img src="./assets/icons/FHIR/Intro2.png" width="40%"/>](#2-)

[3. <img src="./assets/icons/FHIR/Intro3.png" width="40%"/>](#3-)

[4. <img src="./assets/icons/FHIR/Intro4.png" width="40%"/>](#4-)

[5. <img src="./assets/icons/FHIR/Intro5.png" width="40%"/>](#5-)

---

## 1. <img src="./assets/icons/FHIR/Intro1.png" width="70%"/>

FHIRデータ標準を利用することで相互運用性をどのように向上させることができるか、ビデオを利用してを学習します。

- HL7 FHIR とは？

    >日本語吹き替えできたら置き換える

    {% include youtube.html id="AkqNuxVBQKY" %}


- 日本語字幕付きビデオ「FHIR - 未来のために設計された医療データスタンダード "FHIR A Healthcare Data Standard Designed for the Future"

    {% include youtube.html id="gNjlaARboYk" %} 


---

## 2. <img src="./assets/icons/FHIR/Intro2.png" width="70%"/>

HL7® FHIR® ヘルスケアデータ標準の概要と、ウェブサイトのナビゲート方法を学習します。

また、FHIRの目標、データの保存と共有方法の基本、仕様内のさまざまなFHIRリソース間の関係について学習します。

- FHIRとは何か、現在、そして今後

    このビデオは、国際モダンホスピタルショウ2022 インタ―システムズブースのミニシアターで開催された　一般社団法人 日本IHE協会　理事　接続検証委員長　塩川 康成 様　によるご講演ビデオです。

   >国際モダンホスピタルショウ　インタ―システムズブースのミニシアターでのご講演内容全般については、[InterSystems Japan YouTubeチャンネル](https://www.youtube.com/@InterSystemsJapan/playlists)にて公開しております。

    {% include youtube-list.html id="_Qgv9WqrN6k" list="PLgFt3CvX3OePAiRdrL8GmMzKNiCG_BJqP" %}


> **英語ビデオもあります**
>
>- [ビデオ（英語）：What Is the HL7 FHIR Specification?](https://www.youtube.com/watch?v=OAS2mp-6TXY&list=PLp4xNHWZ7IQkqH6bHsYVFkh1tX0P1_2VF&index=3)
>
>- [ビデオ（英語）：Organizing HL7 FHIR Resources](https://www.youtube.com/watch?v=-dcaWj1gZSo&list=PLp4xNHWZ7IQkqH6bHsYVFkh1tX0P1_2VF&index=4)
{: .block-tip}

---
## 3. <img src="./assets/icons/FHIR/Intro3.png" width="70%"/>
個々のFHIRリソースの構造、データ表現の一貫性を可能にするデータ型と用語バインディングについて、FHIR標準仕様のウェブサイトを使用しながら確認します。

- ビデオ（英語）：Understanding the Structure of HL7 FHIR Resources

    HL7® FHIR® リソースの構造を紹介します。
    
    [FHIR ウェブサイト](https://hl7.org/fhir/R4/)のリソースのツリー表示の見方と読み方を確認し、リソースに含まれる様々なデータ要素を理解します。
    
    また、リソースを XML、JSON、または Turtle で表示する方法や、FHIR リソースの UML (Universal Modeling Language) ダイアグラムの場所についても説明します。

    {% include youtube-list.html id="BmgAhxWQtZw" list="PLp4xNHWZ7IQkqH6bHsYVFkh1tX0P1_2VF" %}


- ビデオ（英語）：Identifying Structured and Coded Data in HL7 FHIR Resources

    HL7® FHIR® で使用され、データセットの表現に一貫性を持たせる、構造化データとコード化データの識別方法を学習できます。
    
    FHIR で使用されるデータ型と、用語バインディングが要素定義をデータ型と値セットにどのように結びつけるかを確認できます。
    
    また、FHIRリソースの一部として定義されたコードや、LOINCやSNOMEDのような外部の用語体系から引き出されたコードの例をご覧ください。

    {% include youtube-list.html id="D8QafQ6-yZw" list="PLp4xNHWZ7IQkqH6bHsYVFkh1tX0P1_2VF" %}

---
## 4. <img src="./assets/icons/FHIR/Intro4.png" width="70%"/>

FHIRプロファイルと実装ガイド、FHIR shorthand を詳しく確認し、FHIRデータアーキテクチャを理解します。

>全て英語。日本語字幕を付けたらいいのか。他で代用できるものがあるのか。

- FHIRプロファイルについて

    {% include youtube-list.html id="B-B6ge_0nHg" list="PLzSN_5VbNaxBu4kMgZrK5iGi-GIGNxvpu&index=8" %}

> **英語ビデオあります**
>
>- [ビデオ（英語）:Understanding HL7 FHIR Profiles](https://youtu.be/YHVlghfGsq4?list=PLp4xNHWZ7IQkqH6bHsYVFkh1tX0P1_2VF)
{: .block-tip}

- FHIR実装ガイドについて（英語ビデオ）

    {% include youtube-list.html id="AfoXYVgzE9U" list="PLp4xNHWZ7IQkqH6bHsYVFkh1tX0P1_2VF" %}

- FHIR Shorthandについて

    HL7® FHIR® Shorthand を使用して FHIR 実装ガイドをより効率的に作成する方法を学習します。 
    
    FHIR Shorthand は、プロファイル、エクステンション、およびその他の FHIR アーティファクトを定義するための、ドメイン固有の人間が読める言語です。

    - 記事：[SUSHIを使ってFHIRプロファイルを作成しようパート1](https://jp.community.intersystems.com/node/493351)

    - 記事：[SUSHIを使ってFHIRプロファイルを作成しようパート2](https://jp.community.intersystems.com/node/506271)


> **英語ビデオあります**
>- [ビデオ（英語）：Using HL7 FHIR Shorthand](https://www.youtube.com/watch?v=_vakrZk482k&list=PLp4xNHWZ7IQkqH6bHsYVFkh1tX0P1_2VF&index=9)
{: .block-tip}


- [演習環境付き演習（英語）のオンラインコース：Building a FHIR Data Architecture](https://learning.intersystems.com/course/view.php?id=2279)

    HL7® FHIR® アーキテクチャとその基礎となるデータモデルの基礎を学びます。
    
    この演習では、InterSystems がサポートする Graph Builder 2 (GB2) アプリを使用して、FHIR を使用した開発の基礎となる FHIR データアーキテクチャの構築を開始します。

---

## 5. <img src="./assets/icons/FHIR/Intro5.png" width="70%"/>
医療システム間のセマンティック相互運用性について学び、FHIR分野で最もよくある質問を確認します。

- （ビデオ：英語）[Achieving True Interoperability in Healthcare Systems](https://learning.intersystems.com/course/view.php?id=2203) 
    
    セマンティック相互運用性の概念と、医療データ交換におけるその役割についてご紹介します。
    
    セマンティック相互運用性は、医療データが確実に伝送されるだけでなく、容易に理解されることを保証するために、システムマッピングを超えるものです。HL7® FHIR® データ標準がこの課題にどのように対応できるかを紹介します。
    
    >同じ病名疑いでもそれぞれの病院で記載される書かれ方はそれぞれ。それを同じであるとみなすことはシステムだけではできない。FHIRのプロファイルを使って当てはめれば違うEHRの書き方でも統一できるよ。的な内容。人の確認も必要よ

    {% include youtube-list.html id="us6W4ppN9SA" list="PLp4xNHWZ7IQkqH6bHsYVFkh1tX0P1_2VF&index=11" %} 


- （ビデオ：英語）FHIR FAQs

    InterSystems のSenior Clinical Interoperability Advisor である Russ Leftwich が HL7® FHIR® に関してよくある質問に回答します。

    {% include youtube-list.html id="tH2sWhVa8MU" list="PLp4xNHWZ7IQkqH6bHsYVFkh1tX0P1_2VF&index=10" %} 
