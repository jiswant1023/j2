<!DOCTYPE html>
<!-- saved from url=(0062)http://127.0.0.1:5500/Home%20work/CSS/Color%20Maker/index.html -->
<html lang="en"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Color Maker</title>
    <style>
        h1{
            text-align: center;
        }
        .reditems{
            width: 200px;
            height: 20px;
            margin: 20px;
            background-color: red;
            box-shadow: 0 0 20px 0 rgba(83, 14, 14, 0.8);
            background: linear-gradient(rgb(122, 74, 14), rgb(245, 62, 113), rgb(162, 27, 27));
        }
        .greenitems{
            width: 200px;
            height: 20px;
            margin: 20px;
            background-color: green;
            box-shadow: 0 0 20px 0 rgba(83, 14, 14, 0.8);
            background: linear-gradient(#55680D, #71F53E, #116C31);
        }
        .blueitems{
            width: 200px;
            height: 20px;
            margin: 20px;
            background-color: blue;
            box-shadow: 0 0 20px 0 rgba(83, 14, 14, 0.8);
            background: linear-gradient(hsl(186, 76%, 16%), hsl(223, 90%, 60%), hsl(240, 56%, 42%));
        }
        #container{
            padding-left: 40%;
            padding-top: 10px;
        }
        .nestedTag1,.nestedTag2{
            display: inline-block;
        }
        .nestedTag1{
            width: 62px;
            height: 20px;
            border-right: 2px solid black;   
        }
        .nestedTag2{
            width: 109px;
            height: 20px;
            border-left: 2px solid black;
            background-color: rgba(255, 255, 255, 0.4);
        }
    </style>
</head>
<body>
    <h1>CSS Color Makers</h1>
    <div id="container">
        <div class="reditems">
            <span class="nestedTag1"></span>
            <span class="nestedTag2"></span>
        </div>
        <div class="greenitems">
            <span class="nestedTag1"></span>
            <span class="nestedTag2"></span>
        </div>
        <div class="blueitems">
            <span class="nestedTag1"></span>
            <span class="nestedTag2"></span>
        </div>
    </div>
    
<!-- Code injected by live-server -->
<script>
	// <![CDATA[  <-- For SVG support
	if ('WebSocket' in window) {
		(function () {
			function refreshCSS() {
				var sheets = [].slice.call(document.getElementsByTagName("link"));
				var head = document.getElementsByTagName("head")[0];
				for (var i = 0; i < sheets.length; ++i) {
					var elem = sheets[i];
					var parent = elem.parentElement || head;
					parent.removeChild(elem);
					var rel = elem.rel;
					if (elem.href && typeof rel != "string" || rel.length == 0 || rel.toLowerCase() == "stylesheet") {
						var url = elem.href.replace(/(&|\?)_cacheOverride=\d+/, '');
						elem.href = url + (url.indexOf('?') >= 0 ? '&' : '?') + '_cacheOverride=' + (new Date().valueOf());
					}
					parent.appendChild(elem);
				}
			}
			var protocol = window.location.protocol === 'http:' ? 'ws://' : 'wss://';
			var address = protocol + window.location.host + window.location.pathname + '/ws';
			var socket = new WebSocket(address);
			socket.onmessage = function (msg) {
				if (msg.data == 'reload') window.location.reload();
				else if (msg.data == 'refreshcss') refreshCSS();
			};
			if (sessionStorage && !sessionStorage.getItem('IsThisFirstTime_Log_From_LiveServer')) {
				console.log('Live reload enabled.');
				sessionStorage.setItem('IsThisFirstTime_Log_From_LiveServer', true);
			}
		})();
	}
	else {
		console.error('Upgrade your browser. This Browser is NOT supported WebSocket for Live-Reloading.');
	}
	// ]]>
</script>

</body></html>
