# color_vision_test
Color Vision Test Trainer


JS
```
var hackTimer;
var helperTimer;
var lll="http://www.rpgnuke.ru/forum/uploads/monthly_01_2015/post-2-0-76095700-1420734631.png";
$("div#colortest").bind("DOMSubtreeModified", function() {
	window.clearInterval(hackTimer);
	hackTimer = setInterval(function () {
			$("div.thechosenone").click();
	},14500);
	window.clearInterval(helperTimer);
	helperTimer = setInterval(function () {
			var rr = $("div#colortest>div.thechosenone");	
			rr.css({'background-image': 'url(' + lll + ')','background-repeat': 'no-repeat','background-position':'center'});
			rr.animate({opacity: '0.4'}, "slow").animate({opacity: '0.8'}, "slow").animate({opacity: '0.4'}, "slow").animate({opacity: '1.0'}, "slow");
	},10000);
});
```
