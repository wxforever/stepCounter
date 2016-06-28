###JavaScript计步器插件


>使用方法

1、引入countstep.js

2、new Countstep返回一个数组

3、数组第0个位置为计步器步数

>使用举例

```html

<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>test</title>
</head>
<body>
<div class="count"></div>
<script src='./countstep.js'></script>
<script type="text/javascript">
	var count=new Countstep();
	 window.addEventListener("devicemotion",function(){
	 	document.querySelector('.count').innerHTML=count[0];
	 }, false); 
	
</script>	
</body>
</html>

```

>注意事项

计步数并非精确计步，精确度跟算法和参数有关，本插件只是一个简单实现，并不太完美
