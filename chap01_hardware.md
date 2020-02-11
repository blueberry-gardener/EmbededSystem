<script type="text/x-mathjax-config">MathJax.Hub.Config({tex2jax:{inlineMath:[['\$','\$'],['\\(','\\)']],processEscapes:true},CommonHTML: {matchFontHeight:false}});</script>
<script type="text/javascript" async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-MML-AM_CHTML"></script>
<script type="text/x-mathjax-config">MathJax.Hub.Config({displayAlign: "left",displayIndent: "2em"});</script>

<style>
body {
    counter-reset: h1;
}
h1 {
    counter-reset: h2;
}
h2 {
    counter-reset: h3;
}
h1:before {
    counter-increment: h1;
    content: counter(h1) ". ";
}
h2:before {
    counter-increment: h2;
    content: counter(h1) "." counter(h2) ". ";
}
h3:before {
    counter-increment: h3;
    content: counter(h1) "." counter(h2) "."counter(h3) ". ";
}
</style>

# Hardware

## 論理回路

### 組み合わせ論理回路

#### ド・モルガンの法則

$$
\overline{A・Ｂ} = \bar{A} + \bar{B} \\
\overline{A+Ｂ} = \bar{A} ・ \bar{B}
$$

<div align="center"><img src="./images/01_hardware-dmol.png"  title="aaa"></div>


#### スリーステートバッファ

入力と出力のほかに出力の可否を制御する信号を持つゲート

<div align="center"><img src="./images/01_hardware-3state.png"  title="aaa"></div>

|IN|ENB|OUT|
|--|--|--|
|0|0|Z|
|0|1|0|
|1|0|Z|
|1|1|1|

※Zは、ハイインピーダンスを表す。(信号の衝突を避けるために用いる)

#### オープンドレインとオープンソース

インバータを構成する2個のトランジスタのうち、1個のみを利用する。
<div align="center"><img src="./images/01_hardware-opend.png"  title="aaa"></div>

### 順序論理回路

#### ラッチ
1ビットの情報を保持できる状態を有する電子回路のこと。

<b><font color="#ff0000">【TBW】RSラッチ</font></b>

<b><font color="#ff0000">【TBW】Dラッチ</font></b>

#### フリップフロップ
1ビットの情報を一時的に"0"または"1"の状態として保持することができる論理回路のこと。

<b><font color="#ff0000">【TBW】Dフリップフロップ</font></b>

<b><font color="#ff0000">【TBW】JKフリップフロップ</font></b>


### 加算器

### カウンタ

### タイマ

#### ウォッチドックタイマ
システムの誤操作によってプログラムが正常に実行できなくなったことを検出し、システムをリセットするために用いるタイマ。指定時間が経過してタイムアウトが発生するとシステムをリセットするようなハードウェアタイマを設定しておく。

## アナログ回路

### AD変換

### DA変換

### 積分回路・微分回路

<div align="center"><img src="./images/01_hardware-integral.png"  title="aaa"></div>

### 演算増幅器

### PWN：Pulse Width Modulation：パルス幅変調

### PLL：Phase Locked Loop：位相ロックループ
入力された周波数を逓倍する回路である。


<div align="center"><img src="./images/01_hardware-pll.png"  title="aaa"></div>

## LSI

## メモリ

***
[TopPage](./README.md)