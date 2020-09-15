<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="utf-8">
<title>Limdaun</title>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/Swiper/4.5.1/css/swiper.min.css">
<script src="http://code.jquery.com/jquery-latest.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/Swiper/4.5.1/js/swiper.min.js"></script>

<style>

.box {
	width:100%;
	height:700px;
	background:url(images/sky.jpg);
	background-size: 100%;
	padding-top:100px;
	
}

.box-content {
	color:white;
}

.swiper-container {
	width:1000px;
	height:600px;
	border:2px solid #2E9AFE;
	border-radius:5px;
	background-color:white;
}

.swiper-slide {
	text-align:center;
	display:flex;
	align-items:center;
	justify-content:center;
}

.swiper-slide img {
	width:800px;
	height:480px;
}

</style>

</head>

<body>
	<!-- Swiper 시작 -->
	<div class="box">
		<div class="box-content"></div>
		<div class="swiper-container">
			<div class="swiper-wrapper">
				<div class="swiper-slide" style="font-size:50px; color:#2E9AFE">Daun's Photo Album</div>
				<div class="swiper-slide"><img src="images/sky.jpg"></div>
			</div>

			<!-- 네비게이션 버튼 -->
			<div class="swiper-button-next"></div><!-- 다음 버튼 -->
			<div class="swiper-button-prev"></div><!-- 이전 버튼 -->

			<!-- 페이징 -->
			<div class="swiper-pagination"></div>
		</div>
	</div>

<script>

new Swiper('.swiper-container', {
	pagination : { // 페이징 설정
		el : '.swiper-pagination',
		clickable : true, // 페이징을 클릭하면 해당 영역으로 이동, 필요시 지정해 줘야 기능 작동
	},
	navigation : { // 네비게이션 설정
		nextEl : '.swiper-button-next', // 다음 버튼 클래스명
		prevEl : '.swiper-button-prev', // 이번 버튼 클래스명
	},
	autoplay: {
    delay: 3000, // 3초 자동 재생
  	},
});

</script>
</body>
</html>
