
https://jquerymobile.com/

<!DOCTYPE html>
<html lang="zh">
<head>
	<meta charset="UTF-8" />
	<title>Document</title>
</head>
<body>
	<div id="app"></div>
<script src="jquery-3.2.1.js" type="text/javascript" charset="utf-8"></script>
<script type="text/javascript">
	
	/*
		插件、组件
		
		插件:辅助型的
		组件:独立的功能型
		
		
		JQ用以下的方法来扩展插件
		
		$.extend();
		
		$.fn.extend();
		
		
		工具方法:
			$.ajax()
			
			$.each()
		
		功能方法
			
			$('box').hide();
			$('box').show();
			
		
		
		$.extend(true,{},{})
		
			可以浅拷贝
			深拷贝
			还能写插件
		
		
	*/
	
	
	var str = '    sadsda     ';
	
	$.extend({
		leftTrim:function(str){
			return str.replace(/^\s+/,'');
		}
	});
	
	
	
	$.fn.extend({
		
		red:function(){
			//this,为调用这个方法的JQ对象
			///console.log(this); //#app
			
			this.css({
				width:100,
				height:100,
				background:'red'
			});
			
			return this;
			
		}
		
	});
	
	$('#app').red();
	
//	.css({
//		border:'10px solid #000'
//	});
	
	
	
	
//	console.log($.leftTrim(str));
	
	
	
	
</script>
</body>
</html>
