# CTFd writeups

*	[Misc - easy wireshark (50)](#easy_wireshark)
*	[Crypto - easy! (50)](#easy!)
*	[Crypto - keyboard (100)](#keyboard)
*	[Crypto - n 次 base64 (200)](#n次base64)
*	[隱寫術 - 女神 (50)](#女神)



<h2 id="easy_wireshark">Misc - easy wireshark (50)</h2>

> wireshark.pcapng

hint: 听说抓到他浏览网页的包,flag就在网页里

用 wireshark 開 .pcapng，export HTTP

就有一個檔案叫 flag.php

<h2 id="easy!">Crypto - easy! (50)</h2>

bmN0Znt0aGlzX2lzX2Jhc2U2NF9lbmNvZGV9

base64


<h2 id="keyboard">Crypto - keyboard (100)</h2>

ytfvbhn tgbgy hjuygbn yhnmki tgvhn uygbnjm uygbn yhnijm

areuhack

<h2 id="n次base64">Crypto - n 次 base64 (200)</h2>

> base64.txt

跑幾圈隨便設定，跳出 error 就表示次數太多

```python
#!usr/bin/env python
import base64

p = [題目]

for i in range(1, 50):
	p = base64.b64decode(p)
	print p
```
次數剩很少時直接用線上 decode
`flag:nctf{please_use_python_to_decode_base64}`

<h2 id="女神">隱寫術 - 女神 (50)</h2>

> misc1.jpg

用記事本打開圖檔

`nctf{pic_yin_xie_shu}`