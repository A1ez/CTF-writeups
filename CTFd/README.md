# CTFd writeups


*	[Misc - easy wireshark (50)](#easy_wireshark)
*	[Web - AAencode (100)](#AAencode)
*	[Crypto - easy! (50)](#easy!)
*	[Crypto - keyboard (100)](#keyboard)
*	[Web - php decode (100)](#php_decode)
*	[Web - 簽到 2 (50)](#簽到2)
*	[Crypto - n 次 base64 (200)](#n次base64)
*	[Web - 這題不是 Web (100)](#這題不是Web)
*	[Web - 單身二十年 (100)](#單身二十年)
*	[隱寫術 - 女神 (50)](#女神)
*	[Web - 你從哪裡來 (100)](#你從哪裡來)
*	[Web - 層層地進 (100)](#層層地進)
*	[Web - 單身一百年也沒用 (150)](#單身一百年也沒用)
*	[Web - Download~! (200)](#Download~!)
*	[Web - md5 collision (50)](#md5_collision)


<h2 id="easy_wireshark">Misc - easy wireshark (50)</h2>

> wireshark.pcapng

hint: 听说抓到他浏览网页的包,flag就在网页里

用 wireshark 開 .pcapng，export HTTP

就有一個檔案叫 flag.php

<h2 id="AAencode">Web - AAencode (100)</h2>

> aaencode.txt

AAencode 是把 JavaScript 加密成表情符號的加密法

decode >> alert("Hello, JavaScript")

在 chrome console 送，就會直接跑出那個對話框

直接把整串亂七八糟的符號送出去，得到 flag

<h2 id="easy!">Crypto - easy! (50)</h2>

bmN0Znt0aGlzX2lzX2Jhc2U2NF9lbmNvZGV9

base64


<h2 id="keyboard">Crypto - keyboard (100)</h2>

ytfvbhn tgbgy hjuygbn yhnmki tgvhn uygbnjm uygbn yhnijm

areuhack


<h2 id="php_decode">Web - php decode (100)</h2>

```php
<?php
function CLsI($ZzvSWE) {
    $ZzvSWE = gzinflate(base64_decode($ZzvSWE));
    for ($i = 0; $i < strlen($ZzvSWE); $i++) {
        $ZzvSWE[$i] = chr(ord($ZzvSWE[$i]) - 1);
    }
    return $ZzvSWE;
}eval(CLsI("+7DnQGFmYVZ+eoGmlg0fd3puUoZ1fkppek1GdVZhQnJSSZq5aUImGNQBAA=="));?>
```

改成

```php
<?php
function CLsI($ZzvSWE) {
    $ZzvSWE = gzinflate(base64_decode($ZzvSWE));
    for ($i = 0; $i < strlen($ZzvSWE); $i++) {
        $ZzvSWE[$i] = chr(ord($ZzvSWE[$i]) - 1);
    }
    return $ZzvSWE;
}
echo CLsI("+7DnQGFmYVZ+eoGmlg0fd3puUoZ1fkppek1GdVZhQnJSSZq5aUImGNQBAA==");
?>
```

得到
`phpinfo(); flag:nctf{gzip_base64_hhhhhh}`


<h2 id="簽到2">Web - 簽到 2 (50)</h2>

```html
<form action="./index.php" method="post">
	<p>输入框：<input type="password" value="" name="text1" maxlength="10"><br>
	请输入口令：zhimakaimen
	<input type="submit" value="开门">
</form>
```

長度限制 10，`zhimakaimen`長度 11

firefox - HackBar - Enable Post data

`text1=zhimakaimen`

`nctf{follow_me_to_exploit}`


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


<h2 id="這題不是Web">Web - 這題不是 Web (100)</h2>

> 2.gif

用 .txt 開啟

`nctf{photo_can_also_hid3_msg}`


<h2 id="單身二十年">Web - 單身二十年 (100)</h2>

用 burp 看到 (chrome 的 network 也可以看到)

> GET /web8/no_key_is_here_forever.php HTTP/1.1
> 
> Host: chinalover.sinaapp.com
> 
> User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64; rv:47.0) Gecko/20100101 Firefox/47.0
> 
> Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
> 
> Accept-Language: zh-TW,zh;q=0.8,en-US;q=0.5,en;q=0.3
> 
> Accept-Encoding: gzip, deflate
> 
> Referer: http://chinalover.sinaapp.com/web8/search_key.php
> 
> Connection: close

Action -> Sent to Repeater 改成

> GET /web8/search_key.php HTTP/1.1

送回去

Response

```php
<script>window.location="./no_key_is_here_forever.php"; </script>
key is : nctf{yougotit_script_now}
```

<h2 id="女神">隱寫術 - 女神 (50)</h2>

> misc1.jpg

用記事本打開圖檔

`nctf{pic_yin_xie_shu}`


<h2 id="你從哪裡來">Web - 你從哪裡來 (100)</h2>

HTTP Header 有一個叫 Referer

> Referer：表示瀏覽器所存取的前一個頁面，正是那個頁面上的某個連結將瀏覽器帶到了當前所請求的這個頁面。

用 burp 補上

```
Referer: google.com
```

`flag:nctf{http_referer}`


<h2 id="層層地進">Web - 層層地進 (100)</h2>

偷看別人的 writeups 才知道要訪問 http://chinalover.sinaapp.com/web3/404.html

原始碼中間有一段

```php
<!-- Placed at the end of the document so the pages load faster -->
<!--  
<script src="./js/jquery-n.7.2.min.js"></script>
<script src="./js/jquery-c.7.2.min.js"></script>
<script src="./js/jquery-t.7.2.min.js"></script>
<script src="./js/jquery-f.7.2.min.js"></script>
<script src="./js/jquery-{.7.2.min.js"></script>
<script src="./js/jquery-t.7.2.min.js"></script>
<script src="./js/jquery-h.7.2.min.js"></script>
<script src="./js/jquery-i.7.2.min.js"></script>
<script src="./js/jquery-s.7.2.min.js"></script>
<script src="./js/jquery-_.7.2.min.js"></script>
<script src="./js/jquery-i.7.2.min.js"></script>
<script src="./js/jquery-s.7.2.min.js"></script>
<script src="./js/jquery-_.7.2.min.js"></script>
<script src="./js/jquery-a.7.2.min.js"></script>
<script src="./js/jquery-_.7.2.min.js"></script>
<script src="./js/jquery-f.7.2.min.js"></script>
<script src="./js/jquery-l.7.2.min.js"></script>
<script src="./js/jquery-4.7.2.min.js"></script>
<script src="./js/jquery-g.7.2.min.js"></script>
<script src="./js/jquery-}.7.2.min.js"></script>
-->
```

還是不知為何要訪問 `/404.html`

`nctf{this_is_a_fl4g}`


<h2 id="單身一百年也沒用">Web - 單身一百年也沒用 (150)</h2>

chrome - Network

有個被重新導向的 index.php

他的 Response Header `flag:nctf{this_is_302_redirect}`


<h2 id="Download~!">Web - Download~! (200)</h2>

提示說想下啥就下啥，但別下載音樂...

注意到兩首歌的 url

```
download.php?url=eGluZ3hpbmdkaWFuZGVuZy5tcDM=
download.php?url=YnV4aWFuZ3poYW5nZGEubXAz
```
把兩串都拿去 base64 decode，發現都是該檔檔名

xingxingdiandeng.mp3

buxiangzhangda.mp3

也就是說把想下載的檔名拿去 base64 encode 就可以下載了

直接在網頁上訪問 download.php

```
?Access Forbidden!
```

只好把他下載下來

```
base64('download.php') = ZG93bmxvYWQucGhw
download.php?url=ZG93bmxvYWQucGhw
```

download.php

```php
??<?php
error_reporting(0);
include("hereiskey.php");
$url=base64_decode($_GET[url]);
if( $url=="hereiskey.php" || $url=="buxiangzhangda.mp3" || $url=="xingxingdiandeng.mp3" || $url=="download.php"){
	$file_size = filesize($url);
	header ( "Pragma: public" );
	header ( "Cache-Control: must-revalidate, post-check=0, pre-check=0" );
	header ( "Cache-Control: private", false );
	header ( "Content-Transfer-Encoding: binary" );
	header ( "Content-Type:audio/mpeg MP3");
	header ( "Content-Length: " . $file_size);
	header ( "Content-Disposition: attachment; filename=".$url);
	echo(file_get_contents($url));
	exit;
}
else {
	echo "Access Forbidden!";
}
?>
```

有個檔案叫 `hereiskey.php`，下載他

```php
?<?php
//flag:nctf{download_any_file_666}
?>
```

<h2 id="md5_collision">Web - md5 collision (50)</h2>

```php
<?php
$md51 = md5('QNKCDZO');
$a = @$_GET['a'];
$md52 = @md5($a);
if(isset($a)){
if ($a != 'QNKCDZO' && $md51 == $md52) {
    echo "nctf{*****************}";
} else {
    echo "false!!!";
}}
else{echo "please input a";}
?>
```

```
md5('QNKCDZO') = 0e830400451993494058024219903391
```

覺得漏洞應該在 `==`

但不知道怎麼繞過他

看 writeup 後發現只要是 `0e` 開頭，判別都會過

**但還沒有很清楚為什麼只要 `0e`就過**

找一個做完 md5 後開頭是 0e 的值 `s1091221200a`

```
?a=s1091221200a
```

`nctf{md5_collision_is_easy}`