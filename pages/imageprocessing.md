
[index](https://github.com/kitasenjudesign/CreativeCodingDictionary/blob/master/README.md)

# ■変換

### アフィン変換
平行移動拡大縮小、平行四辺形的変換が可能。台形はできない。
3x3の行列であらわされる。
http://imagingsolution.blog107.fc2.com/blog-entry-284.html

### 射影変換（ホモグラフィ）
台形もできる。アフィン変換と同様に、行列で計算できる。

### 細線化アルゴリズム
http://imagingsolution.blog107.fc2.com/blog-entry-138.html
太い絵から線を抽出する方法があるらしい。

### ハフ変換
https://qiita.com/YSRKEN/items/ee94c7c22599c2374722

# ■フィルタ

### ガウシアン

### ラプラシアン
3x3で 0,-1,0, -1,4,-1, 0,-1,0 という係数を持ち、エッジ抽出に使われる。空間の２回微分なので微分方程式とかにも出てくる。
2次微分のかたちなのでノイズが強調されることがある。
2次微分なのでゼロ交差をエッジの位置とする。


### LOG ( ラプラシアンオブガウシアン　）
ガウスをかけた後、ラプラシアンをかけるとノイズも消える。ボケ次第で、いろんなエッジがとれる。
http://mainly-coding.blogspot.jp/2009/06/17-log.html


### sobel
綺麗にエッジ抽出できる。

### メディアン
中央値を取るフィルタで、エッジを保持しつつ、インパルスを消す。

### ディザ
ディザ（Dither）とは、量子化誤差（端数）を、単純に丸めるのではなく、全体の量子化誤差が最小化するよう確率を調整して切り捨てまたは切り上げのどちらかをランダムにおこなうためによるゆらぎのことである。そのような一種のノイズ的データを追加する作業および技法はディザリング（Dithering）またはディザ法と呼ばれる。誤差を周囲のデータに拡散する手法をも含めて言うこともある。

### 2値化(ランダムディザ)
閾値を乱数できめる。
https://ics.media/entry/5535

### 2値化(ベイヤーディザ)
4px x 4pxから決める。

### エンボス
画像A　を　ネガポジ反転したのち　ちょい平行移動したA' があったとすると
A + A' - 128
で得られる結果。変化がない部分は128の灰色、変化がある部分は白か黒になる。


# ■動画
### オプティカルフロー
ブロックマッチング法、勾配法

### 移動体追跡

# ■圧縮
###  

### 

# 
