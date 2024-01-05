<html>
<head>
	<title>GDC Banners</title>
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<meta name="robots" content="noindex" />
	<link rel="icon" href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAEzSURBVHgBrVZbEYQwDFwJSIgEJJwEJJyDwwF1Ag6QgBQkIIFruYS2DKQt3M7kpzSvzaMAOiornZXJymxlZVn4rLVCuAFiA2um9Chw9OEIJVKn3BwM1Hw2IM6qTRnvAoURP4pSoIOjDkrkcikZyQmMpk/wtBjcRwtPF4UfevhiPcXItiY5IPjU6EKppEtc3YSNrYaSlhZ9aTsOCOiWfm8yHDiZrbyho0FAk6RTZzrIcUTBnV0BhQ5StO12nzq4muDd7gy9g6AYNjif9jq4U1zkVTEsiIps8P82lcHdqKvg07mKykXyQh4IJ4MrNI14jtO1Q/DzcGeTCjpcLDvArwx1pyvIWvcG5QV1dRsRd5gK5305OHJtF64S4rMe8fOaTS8hfgZTMuHB30XLBsKsZj4zSLzbX4x4t71zkqRYAAAAAElFTkSuQmCC">
</head>
<body class="no-js">
	
	<div id="adblocker" class="adblocker">It looks like you're using an ad blocker, which <em>may</em> cause some banner previews to break or not show up properly.</div>
	<div id="grid" class="grid">
		<div class="col">
			<div class="wrapper" style="width: 120px; height: 600px; background-color: #000000;"><h6 class="heading" style="width: 120px;">120x600</h6>
				<iframe
					title="120x600 Skyscraper"
					width="120"
					height="600"
					src="banners/120x600_Skyscraper/index.html"
					frameBorder="0"></iframe></div>
		</div>
		<div class="col">
			<div class="wrapper" style="width: 320px; height: 50px; background-color: #000000;"><h6 class="heading" style="width: 320px;">320x50</h6>
				<iframe
					title="320x50 Mobile"
					width="320"
					height="50"
					src="banners/320x50_Mobile/index.html"
					frameBorder="0"></iframe></div>
		</div>
		<div class="col">
			<div class="wrapper" style="width: 728px; height: 90px; background-color: #000000;"><h6 class="heading" style="width: 728px;">728x90</h6>
				<iframe
					title="728x90 Leaderboard"
					width="728"
					height="90"
					src="banners/728x90_Leaderboard/index.html"
					frameBorder="0"></iframe></div>
		</div>
		<div class="col">
			<div class="wrapper" style="width: 300px; height: 250px; background-color: #000000;"><h6 class="heading" style="width: 300px;">300x250</h6>
				<iframe
					title="300x250 Medium rectangle"
					width="300"
					height="250"
					src="banners/300x250_Medium_rectangle/index.html"
					frameBorder="0"></iframe></div>
		</div>
	</div>
	<style>
		body {
			background-color: #E5E5E5;
			font-family: 'Helvetica', 'Arial', sans-serif;
			margin: 0;
		}
		.heading {
			font-size: 10px;
			font-weight: normal;
			color: #666;
			margin: 10px 0;
			position: absolute;
			white-space: nowrap;
			overflow: hidden;
			text-overflow: ellipsis;
			top: -25px;
			text-align: left;
		}
		
		.wrapper {
			position: relative;
		}
		
		.grid {
			position: relative;
			z-index: 1;
			margin: 60px 40px;
			text-align: left;
		}
		
		.col {
			display: block;
			margin-bottom: 50px;
		}
		
		.no-js .replay-button {
			display: none;
		}
		
		.adblocker {
			display: none;
			position: fixed;
			right: 24px;
			bottom: 24px;
			margin-left: 24px;
			background-color: #800000;
			padding: 10px;
			font-family: 'Helvetica', 'Arial', sans-serif;
			font-size: 14px;
			border-radius: 4px;
			color: #ffffff;
			z-index: 3;
			box-shadow:
			0 2px 2.7px rgba(0, 0, 0, 0.012),
			0 5px 6.9px rgba(0, 0, 0, 0.018),
			0 10.3px 14.2px rgba(0, 0, 0, 0.022),
			0 21.2px 29.2px rgba(0, 0, 0, 0.028),
			0 58px 80px rgba(0, 0, 0, 0.04);
		}
		.no-js .col {
			display: inline-block;
			vertical-align: top;
			margin: 20px;
			margin-bottom: 50px;
		}
	</style>
	
	<script type="text/javascript">
		document.body.className = "js";
		
		const inViewObserver = new IntersectionObserver(entries => {
			entries.forEach(entry => {
				if (entry.isIntersecting) {
					entry.target.src += '';
				}
			})
		}, { threshold: 0 })
		
		var frames = document.getElementsByTagName('iframe');
		for (var i in frames) {
			try {
				var frame = frames[i];
				inViewObserver.observe(frame);
			} catch(e) {
				console.log(e);
			}
		}
		
	</script><script type="text/javascript" src="https://unpkg.com/masonry-layout@4/dist/masonry.pkgd.js"></script>
	<script type="text/javascript">
		if (window.Masonry) {
			var elem = document.getElementById("grid");
			var msnry = new Masonry(elem, {
				itemSelector: ".col",
				gutter: 20
			});
		}
	</script>
	<script type="text/javascript">
		document.addEventListener('DOMContentLoaded', init, false);
		
		function init(){
			adsBlocked(function(blocked){
				if(blocked){
					document.getElementById('adblocker').style.display = 'block';
				}
			})
		}
		
		function adsBlocked(callback){
			var testURL = 'https://s0.2mdn.net/ads/studio/cached_libs/gsap_3.11.1_min.js'
			
			var init = {
				method: 'HEAD',
				mode: 'no-cors'
			};
			
			var myRequest = new Request(testURL, init);
			
			fetch(myRequest).then(function(response) {
				return response;
			}).then(function(response) {
				callback(false)
			}).catch(function(e){
				callback(true)
			});
		}
	</script>
</body>
</html>
