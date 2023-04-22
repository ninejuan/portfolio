<script>
	export let data;
	</script>

<body style="margin:0; text-align:center;">
	<noscript>엄? 자바스크립트가 작동되지 않네요.</noscript>
	<!-- <nav class="navbar">
		<div class="MainText">
			<a href="/" class="tNoDec tLime">TeamLaon. 주안.</a>
		</div>
	</nav> -->
	<div class="fullscr MidText bBlack">
		<div class="Main">
			<div class="MainText">
                <br><br><br><br><br><br>
				<div class="box fsmain pBorder">
					<img src="assets/profile.png" alt="" class="profile" />
				</div>
			</div>
		</div>
        <br><br>
		<h1 class="tWhite" style="font-size: 60px;">주안</h1>
		<h2 class="tWhite">
			<span>저는 </span>
			<span class="tLime">주안</span>입니다.
		</h2>
        <div class='underLine'><br></div>
	<section class="tMiddle">
		<a name="about"></a>
		<hr style="width: 90vw;">
		<br>
		<div class="intro MPageTxt about">
			<h1 class="tBlack intro" style="font-size: 35px;">
				👋 Hello, World!
			</h1>
			<h2 class="intro">
				학생 풀스택 개발자 겸 화이트해커 주안입니다.<br>
				저는 웹 프레임워크는 SvelteKit과 Express.js를 사용하고 있습니다.<br>
				데이터베이스는 MongoDB를 선호합니다.
			</h2>
		</div>
		<br>
		<a name="skills"></a>
		<hr style="width: 90vw;">
		<div class="skills MPageTxt">
			<h1>
				스킬 Skills
			</h1>
			<img src="assets/language/nodedotjs.png" class="lang" alt="node">
			Node.JS
			<img src="assets/language/typescript.png" class="lang" alt="ts">
			Typescript
			<img src="assets/language/mongodb.png" class="lang" alt="mongo">
			MongoDB
		</div>
		<a name="portfolio"></a>
		<br>
		<hr style="width: 90vw;">
		<div class="projects MPageTxt">
			<h1>
				경력 & 프로젝트 Career & Projects
			</h1>
			<button class="collapsible tBlue tBold">경력 보기</button>
			<div class="CareerContent" style="text-align:center;">
				<div class="defaultCareer">
				<a>{#each data.career.hacking as cr, index}
					<span>{index+1}. {cr}{index === data.career.length - 1 ? '' : ''}</span><br>
				  {/each}</a>
				</div>
				  <div class="minimumCareer">
					<a class="tLime">
						Hacking
					</a><br>
					<a>{#each data.career.hacking as cr, index}
						<span>{index+1}. {cr}{index === data.career.hacking.length - 1 ? '' : ''}</span><br>
					  {/each}</a>
					  <br>
					  <a class="tRed">
						Programming
					  </a><br>
					  <a>{#each data.career.programming as cr, index}
						<span>{index+1}. {cr}{index === data.career.programming.length - 1 ? '' : ''}</span><br>
					  {/each}</a>
				  </div>
			  </div>
			<br><br><br>
			<div class="projectDiv">
				<div class="pIntroBox">
					<img src="assets/portfolio/arambot.png" alt="" width="402" height="213">
					<div class="pIntroText">
						<h2 class="tMiddle subjPj">디스코드 봇, 아람이</h2>
						<p class="tMiddle">아람이는 디스코드 서버 관리 봇입니다. 
							<span class="tOrange">&#60;8/20 운영 종료 예정&#62;</span>
						</p>
					</div>
				</div>
				<br>
				<div class="pIntroBox">
					<img src="assets/portfolio/securelink.png" alt="" width="402" height="213">
					<div class="pIntroText">
						<h2 class="tMiddle subjPj">보안초대링크 오픈소스</h2>
						<p class="tMiddle">디스코드 보안 초대 링크 소스는 <br>
							<a href="https://github.com/Team-Laon/SecureLink" class="tNoDec tLime tBold">여기서</a> 만나보실 수
							있습니다.
							<span class="tRed">&#60;운영 종료&#62;</span>
						</p>
					</div>
				</div>
				<br>
				<div class="pIntroBox">
					<img src="assets/portfolio/aramapi.png" alt="" width="402" height="213">
					<div class="pIntroText">
						<h2 class="tMiddle subjPj">아람이 API</h2>
						<p class="tMiddle">꼭 한번쯤 써봐야 할
							<a href="https://docs.aramy.net" class="tNoDec tLime tBold">API</a>
							<span class="tRed">&#60;운영 종료&#62;</span>
						</p>
					</div>
				</div>
			</div>
		</div>
		<br>
	</section>
	<!-- Channel Plugin Scripts -->
	
	<script src="js/index.js"></script>
	<!-- End Channel Plugin -->
  <footer class="site-footer">
    <div class="container">
      <div class="row">
        <div class="col-sm-12 col-md-3">
          <h6 style="font-family: 'Jua', sans-serif;">정보</h6>
          <p class="text-justify" style="color: gray;">
			초보 화이트해커 주안입니다.
			화이트햇 팀 <a href="https://secstf.kr" target="_blank" rel="noopener noreferrer" style="color:white;text-decoration:none;">SnatchTheFlag</a>에서 활동하고 있습니다.
          </p>
        </div>

        <div class="col-sm-12 col-md-3">
          <h6 style="font-family: 'Jua', sans-serif;">개발</h6>
          <a>
            <img alt="Designed by JuanLee" src="assets/profile.png" width="150" height="150">
          </a>
        </div>

        <div class="col-xs-6 col-md-3">
          <h6>주안Lab</h6>
          <ul class="footer-links">
           <li><a href="https://306.juany.kr" target="_blank" rel="noopener noreferrer">아람이 대시보드</a></li>
            <li><a href="https://docs.aramy.net" target="_blank" rel="noopener noreferrer">아람이 API 문서</a></li>
          </ul>
        </div>

        <div class="col-xs-6 col-md-3">
          <h6>Contact</h6>
          <ul class="footer-links">
            <li><a href="mailto:{data.contact.mail}">Mail</a></li>
            <li><a href="https://github.com/{data.contact.github}" target="_blank" rel="noopener noreferrer">Github</a></li>
            <li><a href="https://discord.com/users/{data.contact.discord}" rel="noopener noreferrer">Discord</a></li>
          </ul>
        </div>
      </div>
      <hr>
    </div>
    <div class="container">
      <div class="row">
        <div class="col-md-8 col-sm-6 col-xs-12">
          <p class="copyright-text">Copyright 2023 <a style="color: lime; text-decoration:none;" href='https://juany.kr' target="_blank" rel="noopener noreferrer">Juan Lee.</a> All Rights Reserved.
          </p>
        </div>
      </div>
    </div>
</footer>
</body>
<slot></slot>
<!-- 폰트 관련

더잠실체
KCC간판체 - 한저위-->