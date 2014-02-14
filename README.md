mbCoimingsoon
=============

Animated responsive countdonw for jQuery.

Getting started 
-----
	<!-- Create a div container -->
	<div id="myCounter"></div>
	
	<!-- Load jQuery -->
	<script src="//ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js"></script>
	<script>
		// If load from CDN fail load jQuery locally
		if (typeof jQuery == 'undefined') {
	            document.write(unescape("%3Cscript src='js/Lib/jquery-1.11.0.min.js' type='text/javascript'%3E%3C/script%3E"));
	        }
	</script>
	
	<script>
		// You have few way to initialize the plugin
		// Passing a Date
		$('#myCounter').mbComingsoon(new Date(2014, 5, 3, 9)) //Expires June 5th 2014 9 o'clock
		//or...
		// Paasing a string (At your own risk!)
		$('#myCounter').mbComingsoon("June 5th 2014") 
		//or
		//Passing an object containing full options
		$('#myCounter').mbComingsoon({
				expiryDate: Date,
				interval: Number, 		//Counter uopdate interval
				localization: {
					days: "days", 		//Localize labels of counter
                                        hours: "hours",
                                        minutes: "minutes",
                                        seconds: "seconds"
				},
				callBack: Function  		//Function executed on expiry or if espired
			}); 
		// Finally you have some additional Methds to control the plugin
		$('#myCounter').mbComingSoon('start') 		// start counter
		$('#myCounter').mbComingSoon('stop') 		// stop counter
		$('#myCounter').mbComingSoon(options: Object) 	// Update options
	</script>

Notes
-----
MbComingsoon is resposive and it is compatible with (<b>but not dependent by</b>) Bootstrap.
MbCaomingsoon dinamically load a subset (only 0-9 characters) of "Open Sans Condensed" Google Font (bold style). If your site already use this font you may comment realated line in mb-comingsoon.less (and recompile) or in css file.

Try a demo <a href="http://jquery.magicbusmultimedia.net">here</a>.
