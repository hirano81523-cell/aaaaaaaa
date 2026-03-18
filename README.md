<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<title>ああああって検索したやつ来い</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body {
  font-family: sans-serif;
  text-align: center;
  background: #111;
  color: #fff;
}

button {
  font-size: 30px;
  padding: 20px;
  margin-top: 30px;
}

#count {
  font-size: 40px;
  margin-top: 20px;
}
</style>
</head>

<body>

<h1>ああああって検索したやつ来い</h1>
<p>暇すぎる人専用ページ</p>

<!-- 広告（あとでAdSense貼る） -->
<div style="margin:20px;">
  広告エリア
</div>

<button onclick="clickCount()">連打しろ</button>
<div id="count">0</div>

<p id="message"></p>

<script>
let count = 0;

function clickCount() {
  count++;
  document.getElementById("count").innerText = count;

  if(count == 10){
    document.getElementById("message").innerText = "まだやるん？";
  }
  if(count == 50){
    document.getElementById("message").innerText = "才能あるで";
  }
  if(count == 100){
    document.getElementById("message").innerText = "人生大丈夫か？";
  }
}
</script>

</body>
</html>
