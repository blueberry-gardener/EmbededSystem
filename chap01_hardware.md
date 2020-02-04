<script type="text/x-mathjax-config">MathJax.Hub.Config({tex2jax:{inlineMath:[['\$','\$'],['\\(','\\)']],processEscapes:true},CommonHTML: {matchFontHeight:false}});</script>
<script type="text/javascript" async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-MML-AM_CHTML"></script>
<script type="text/x-mathjax-config">MathJax.Hub.Config({displayAlign: "left",displayIndent: "2em"});</script>

# 01.Hardware

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

