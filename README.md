# WeatherScraper-
This code is for the Front End design of a weather app. See the Branch for actual code 

<!doctype html>
<html>
<head>
    <title>Alfred's Weather App</title>

<meta charset="utf-8" />
<meta http-equiv="Content-type" content="text/html; charset=utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css" integrity="sha384-rHyoN1iRsVXV4nD0JutlnGaslCJuC7uwjduW9SVrLvRYooPp2bWYgmgJQIXwl/Sp" crossorigin="anonymous">
<style>

 html, body {
 	height:100%;
 }

.container {
			background-image:url("clouds.jpg");
			background-size:cover;	
			background-position:center;
			height:100%;
			width:100%;
			padding-top:150px;
		}

.center {
	text-align:center;
	}
	
.white {
	color:white;
}

button {
	margin-top:20px;
}

h1 {
	padding-bottom:20px;
}

p {
	padding-bottom:20px;
}

.alert {
	margin-top:20px;
	display:none;
}

#success {
	margin-top:20px;
	display:none;
}

#fail {
	margin-top:20px;
	display:none;
}


</style>

</head>

<body>
	
<div class="container">
	<div class="row">
  		<div class="col-md-6 col-md-offset-3 center">
  			
  			<h1 class="center white">Weather App</h1>
  			
  			<p class="lead center white"> Enter your city below </p>
  			
  			<form>
  				
  				<div class="form-group">
  				
  					<input type="text" class="form-control" name="city" id="city" placeholder="Milpitas,CA" />
  				
  				</div>
  				
  				<button id="findMyWeather" class="btn btn-success btn-lg"> Get The Weather</button>
  			
  			</form>	
			
		</div>
	</div>
	
		<div id="success" class="alert alert-success">Success!</div>
		
		<div id="fail" class="alert alert-danger">Failed to retrive weather data!</div>
		
		<div id="noCity" class="alert alert-danger">Please Enter a City</div>
	
</div>

<script src="https://code.jquery.com/jquery-3.1.1.js"   integrity="sha256-16cdPddA6VdVInumRGo6IbivbERE8p7CQR3HzTBuELA="   crossorigin="anonymous"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>


<script>

	$("#findMyWeather").click(function(event) {

		event.preventDefault();
		
			$(".alert").hide();
		
		if ($("#city").val()!="" {
	
			$.get("scraper.php?city="+$("#city").val(), function( data ) {
	
				
				if (data=="") {
					
					$("#fail").fadeIn();
				
					} else {
						
						$("#success").html(data).fadeIn();
				
					}
				});
					} else {
			
						$("#noCity").fadeIn();
					}
				});	



</script>




</body>

</html>
