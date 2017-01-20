# WeatherScraper-
This code is for the Front End design of a weather app. See the Branch for actual code. 

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
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>

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
  				
  				<button class="btn btn-success btn-lg"> Get The Weather</button>
  			
  			</form>	
			
		</div>
	</div>
</div>




</body>

</html>
