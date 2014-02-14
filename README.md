mbCoimingsoon
=============

Animated responsive countdow for jQuery.

Usage 
-----
	<!-- Example -->
	<div id="myCounter"></div>
	
	<script>
		// Passing a Date
		$('#myCounter').mbComingsoon(new Date(2014, 5, 3, 9)) //Expires June 5th 2014 9 o'clock
		
		// Paasing a string (At your own risk!)
		$('#myCounter').mbComingsoon("June 5th 2014") 
		
		//Passing an object
		$('#myCounter').mbComingsoon({
				expiryDate: Date,
				interval: Number, 	//Counter uopdate interval
				localization: {
					days: "days", 	//Localize labels of counter
                                        hours: "hours",
                                        minutes: "minutes",
                                        seconds: "seconds"
				},
				callBack: Function  //Function executed on expiry or if espired
			}); 
	</script>
															}
   Methds:
	.mbComingSoon('start') // start counter
	.mbComingSoon('stop') // stop counter
	.mbComingSoon(options) // Update options
