<!DOCTYPE html>
<html>

  <head>
  
	
    <TITLE>SpaceX Start Coutdown</TITLE>
	<link href="Countdown.css" rel="stylesheet">
	<link href="https://fonts.googleapis.com/css2?family=Gugi&display=swap" rel="stylesheet">
	<link rel="shortcut icon" type="image/x-icon" href="Icon.ico">
	
  </head>

  <body>
	
	<div class="mainpage">
		<div id="mySidenav" class="sidenav">
			<a href="javascript:void(0)" class="closebtn" onclick="closeNav()">&times;</a>
			<a href="#">Über die Mission</a>
			<a href="#">Der Flug</a>
			<a href="#">Die Crew</a>
			<a href="#">Über SpaceX</a>
			<a href="#">Funfackts</a>
		</div>
		
		<div id="main">
			<span onclick="openNav()">&#9776;</span>
		</div>
		
		<script>
			function openNav() {
				document.getElementById("mySidenav").style.width = "250px";
				document.getElementById("main").style.marginLeft = "250px";
				document.body.style.backgroundColor = "rgba(0,0,0,0.4)";
			}
			
			function closeNav() {
				document.getElementById("mySidenav").style.width = "0";
				document.getElementById("main").style.marginLeft= "0";
				document.body.style.backgroundColor = "transparent";
			}
		</script>
		
		<h1>SpaceX Crew Demo-2 Start Coutdown</h1>
		
		<p id="demo"></p>
		
		<script class="CountdownElement">
			// Set the date we're counting down to
			var countDownDate = new Date("May 30, 2020 21:22:45").getTime();
			
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
	</div>
	
	<div>
		<p class="missionText">
			Die Demo-2 Mission ist der letzte Test bevor die</br>
			NASA, SpaceX für bemannte Weltraumflüge ins</br>
			All zertifiziert. Bei der Mission sollen Douglas</br>
			Hurley und Robert Behnken mit einem Dragon 2</br>
			Raumschiff zur ISS gebracht werden.</br>
			Das Ziel der NASA ist es endlich wieder</br>
			bemannten Zugang zum Weltraum zu haben.</br>
			Dieser wurde mit dem Ende des Spaceshuttle-</br>
			Betriebs 2011 geschlossen.
			
		</p>
		
		
		
		
	</div>
	
  </body>
  
</html>
