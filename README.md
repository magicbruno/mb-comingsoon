mb-comingsoon
=============

Animated responsive countdow jQuery plugin.

 Usage: 
   Constructor:
	$(selector).mbComingsoon(expiryDate Date or String) Expiry date of counter
	$(selector).mbComingsoon(options plain Object) options: {
																expiryDate: Date,   //Expiry Date required
																interval: Number,   //Update interval in milliseconds (default = 1000))
                                                                localization: {
                                                                    days: "days",           //Localize labels of counter
                                                                    hours: "hours",
                                                                    minutes: "minutes",
                                                                    seconds: "seconds"
                                                                }
																callBack: Function  //Function executed on expiry or if espired
															}
   Methds:
	.mbComingSoon('start') // start counter
	.mbComingSoon('stop') // stop counter
	.mbComingSoon(options) // Update options
