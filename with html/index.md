<!DOCTYPE HTML>
<html lang ="de-DE">
	<head>
		<title>circle</title>
		<meta charset = "UTF-8" />
		<meta http-equiv="X-UA-Compatible" content="ie=edge">
		<meta name="desciption" content="geometry, circle, sinus, cosinus" >
		<meta name="robots" content="index,follow">
		<meta name="viewport"  content="width=device-width" initial-scale=1.0/>
		<meta name="theme-color" content="#30147e;">
		<link rel ="stylesheet" type="text/css;" href="mobile.css">
		<link rel ="stylesheet" type="text/css;" href="desktop.css">
		<script src="script.js" defer="true"></script>
	</head>
	<body>
		<main class="wrapper">
			<div class="animation">
				<div class="circle">
					<svg class="container" viewBox="-110 -110 220 220">
						<circle cx="0" cy="0" r="100" stroke="blue" stroke-width="3" fill="none"/>
						<line id="x" x1="0" y1="0" x2="100" y2="0" stroke="red" stroke-width="3"></line>
						<line id="y" x1="100" y1="0" x2="100" y2="0" stroke="green" stroke-width="3"></line>
						<line id="vector" x1="0" y1="0" x2="100" y2="0" stroke="orange" stroke-width="3" transform="matrix(1 0 0 1 0 0)"></line>
					</svg>
				</div>
				<div class="rect">
					<svg class="container" viewBox="-110 -110 220 220">
						<rect id="rect" fill="yellow" x="-25" y="-25" width="50" height="50" transform="matrix(1 0 0 1 0 0)"></rect>
					</svg>
				</div>
				<div class="line">
					<svg class="container" viewBox="-110 -110 220 220">
						<line id="line" x1="0" y1="0" x2="100" y2="100" stroke="violet" stroke-width="5" transform="matrix(1 0 0 1 0 0)" />
					</svg>
				</div>
			</div>
			<div class="text"></div>
		</main>
	</body>
</html>