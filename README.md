# hakoniwa

## 概要

[箱庭諸島 S.E ver23_r09](http://hakoniwa.symphonic-net.com/) の改造版

## 「箱庭諸島2 for PHP」のreadme.txtからの引用

> **使用条件**
>
> 箱庭諸島2のスクリプトについては、自己責任で使用する限り、基本的には自由に利用してもらってかまいません。ただし、変更を加えた場合は、変更したものを配布するには、後述の「配布条件」に従って下さい。

> **配布条件**
>
>  箱庭諸島2 for PHPのスクリプトを改変し、それを他人に譲渡、配布する場合には、以下の制約を課します。
>
> ・無料配布であること。  
> ・ゲーム画面のトップに表示される、スクリプトの配布元へのリンクを消すのを禁止すること。また、それ以外の改造は許可すること。  
> ・本条件と同等に、改造したものの配布を許可すること。  
> ・配布するページにおいて、オリジナルスクリプトの配布元として当サイトへのリンクを置くこと。

## 目的/方針

- ナウい環境で実行できるようにする
  - ver.23_r09 は 2013-06-29 で止まっているので古い環境でしか動かない
- 機能はできるだけシンプルにする
  - マニュアルの削除 → 興味のある人は"ググる"だろう
- 画像のローカル設定の削除 → インターネット環境の向上のため
- 「観光者通信」の削除 → メッセージのやりとりはSNSなどを活用する（だろう）


## テスト環境
- Nginx 1.13.2
- PHP 7.4.2

## 変更点

- **バグフィックス**
- **最適化**
- **レガシー対応の削除**
  - HTML5 で廃止される要素の削除
  - 古いIEやNetscapeの対応箇所の削除
  - Chrome, Firefox でも動くように修正
- 日本語変換モジュール(jcode.phps) を廃止 → PHPの関数を利用する
- **コマンドの追加**
  - 「浅瀬埋め立て自動入力」
