# JSDate
Javascript continuous date and time
<!DOCTYPE html>
<html>
<html lang="en-US">
<head>
<title>Simon Kaddissi Web</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="Keywords" content="simon,kaddissi,HTML,CSS,JavaScript,SQL,PHP,jQuery,XML,DOM,Bootstrap,Web development,W3C,tutorials,programming,examples,source code,colors,demos,tips">
<meta name="Description" content="Well organized and easy to understand Web examples of how to use HTML, CSS, JavaScript, SQL, PHP, and XML.">

<style>
#container {width: 100%;}

#head {text-align: center;}

#main p{display: inline-block;
        width: 80px;
        padding: 10px;
        background-color: green;
        color: white;
        font-size: 1.5em;
        text-align: center;}

#main {
        width: auto;
        margin: auto;
        text-align: center;}

</style>
</head>

<body onload=display_ct();>

<div id="container">
<header id="head">
<h1>Simon Kaddissi Web</h1>
<h3>Javascript</hr3>
<h3>setTimeout, onload</h3>
</header>
<hr/>
<p id="full" style="text-align: center;"></p>
<div id="main">


<br/>
<p>year : </p><p id="yr"></p>
<p>month : </p><p id="mt"></p>
<p>day : </p><p id="dy"></p>
<p>time : </p><p id="th"></p>:<p id="tm"></p>:<p id="ts"></p>
<br/>
<!-- <button style = "font-size: 1.5em;" onclick = location.reload(true)>Refresh</button> -->
</div>
<script type="text/javascript">

var timer = null
function display_ct(){
var nd = new Date();

document.getElementById("full").innerHTML = nd;

document.getElementById("yr").innerHTML = nd.getFullYear();

document.getElementById("mt").innerHTML = nd.getMonth();

document.getElementById("dy").innerHTML = nd.getDate();

document.getElementById("th").innerHTML = nd.getHours();

document.getElementById("tm").innerHTML = nd.getMinutes();

document.getElementById("ts").innerHTML = nd.getSeconds();

    timer = setTimeout("display_ct()",1000);
}

</script>

</div>
</body>
</html>
