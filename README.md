# live2d_kbn
看板娘-血小板


```
	<link rel="stylesheet" href="{{ url_for('static',filename='live2d_xxb/css/waifu.css') }}" />
    <script type="text/javascript" src="{{ url_for('static',filename='live2d_xxb/js/live2d.js') }}"></script>
    <script type="text/javascript" src="{{ url_for('static',filename='live2d_xxb/js/waifu.js') }}"></script>
	<div class="waifu ">
	    <div class="waifu-tips" style="opacity:0"></div>
	    <canvas id="live2d" width="200" height="250" class="live2d"></canvas>
	    <div class="live2d_btns">
	    	<i class="fa fa-window-close"></i>
	    </div>
	</div>
	<script type="text/javascript">
	    loadlive2d("live2d", "{{ url_for('static',filename='live2d_xxb/model/kesshouban/model.json') }}");
	    $('.live2d_btns').click(function(){
	    	$('.waifu').hide()
	    })
	</script>
```