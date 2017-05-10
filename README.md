# Parallax-effect

> Parallax effect using Jquery


> # 1. Just write code (HTML):
```s
	<header>
		<div class="header-bg"> </div>
	</header>
```

> # 2. Just write code (CSS):
```s
	<style type="text/css">
		*{
			margin: 0px;
			padding: 0px;
		}
		header{
			position: relative;
			width: 100%;
			height:100vh;
			background-color: #333;
			margin-bottom: 1000px;
			overflow: hidden;
		}
		.header-bg{
			position:absolute;
			width:100%;
			height:300%;
			background-size: 200% 100%;
			background-image: url('img/banner_parallex.jpg');
			background-repeat: no-repeat;
			background-position: center center;
			margin-top: 0px;
		}
	</style>
```

> # 3. Just write code (JavaScript):
```s
	<script type="text/javascript">
		$(window).scroll(function(){
			var scrollTop = $(this).scrollTop();
			$('.header-bg').css('top', -(scrollTop * 2) + 'px');
		})
	</script>
```

> # 4. Then view result in your Browser.
