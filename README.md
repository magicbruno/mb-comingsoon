mbCoimingsoon
=============

Animated responsive countdonw for jQuery.

Usage 
-----
	<!-- Create a div container -->
	<div id="myCounter"></div>
	
	<script>
		// Passing a Date
		$('#myCounter').mbComingsoon(new Date(2014, 5, 3, 9)) //Expires June 5th 2014 9 o'clock
		
		// Paasing a string (At your own risk!)
		$('#myCounter').mbComingsoon("June 5th 2014") 
		
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
		// Additional Methds:
		$('#myCounter').mbComingSoon('start') 		// start counter
		$('#myCounter').mbComingSoon('stop') 		// stop counter
		$('#myCounter').mbComingSoon(options: Object) 	// Update options
	</script>

Notes
-----
MbComingsoon is resposive, is compatible with (<b>but not dipendent by</b>) Bootstrap.
MbCaomingsoon dinamically load a subset (only digits) of "Open Sans Condensed" Google Font (bold style). If your site already use this font you may comment realated line in mb-comingsoon.less (and recompile) or in css file
