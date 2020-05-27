<!DOCTYPE html>
<html>

  <head>
  
	
    <TITLE>SpaceX Start Coutdown</TITLE>
	<link href="Countdown.css" rel="stylesheet">
	<link href="https://fonts.googleapis.com/css2?family=Gugi&display=swap" rel="stylesheet">
	<link rel="shortcut icon" type="image/x-icon" href="Icon.ico">
	
  </head>

  <body>
	
	<div class="navbackground"></div>
	<div class="background"></div>
	
	<h1>SpaceX Crew Demo-2 Start Coutdown</h1>
	
	<p id="demo"></p>
	
	<script class="CountdownElement">
	// Set the date we're counting down to
	var countDownDate = new Date("May 30, 2020 19:22:00").getTime();
	
	// Update the count down every 1 second
	var x = setInterval(function() {
	
	// Get today's date and time
	var now = new Date().getTime();
	
	// Find the distance between now and the count down date
	var distance = countDownDate - now;
	
	// Time calculations for days, hours, minutes and seconds
	var days = Math.floor(distance / (1000 * 60 * 60 * 24));
	var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
	var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
	var seconds = Math.floor((distance % (1000 * 60)) / 1000);
	
	// Display the result in the element with id="demo"
	document.getElementById("demo").innerHTML = days + "d " + hours + "h "
	+ minutes + "m " + seconds + "s ";
	
	// If the count down is finished, write some text
	if (distance < 0) {
		clearInterval(x);
		document.getElementById("demo").innerHTML = "EXPIRED";
	}
	}, 1000);
	</script>

  </body>
  
</html>
