<script>
	import { onMount } from "svelte";

	export let data;
	let s306;
	onMount(() => {
		let r = fetch("http://306.juany.kr")
			.then(() => {
				s306 = true;
			})
			.catch(() => {
				s306 = false;
			});
	});
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
				<br /><br /><br /><br /><br /><br />
				<div class="box fsmain pBorder">
					<img src="/assets/profile.png" alt="" class="profile" />
				</div>
			</div>
		</div>
		<br /><br />
		<h1 class="tWhite" style="font-size: 60px;">주안</h1>
		<h2 class="tWhite">
			<span>저는 </span>
			<span class="tLime">주안</span>입니다.
		</h2>
		<div class="underLine"><br /></div>
		<section class="tMiddle">
			<a name="about" />
			<hr style="width: 90vw;" />
			<br />
			<div class="intro MPageTxt about">
				<h1 class="tBlack intro" style="font-size: 35px;">
					👋 Hello, World!
				</h1>
				<h2 class="intro">
					학생 풀스택 개발자 겸 화이트해커 주안입니다.<br />
					저는 웹 프레임워크는 SvelteKit과 Express.js를 사용하고 있습니다.<br
					/>
					데이터베이스는 MongoDB를 선호합니다.
				</h2>
			</div>
			<br />
			<a name="skills" />
			<hr style="width: 90vw;" />
			<div class="skills MPageTxt">
				<h1>스킬 Skills</h1>
				<img
					src="/assets/language/nodedotjs.png"
					class="lang"
					alt="node"
				/>
				Node.JS
				<img
					src="/assets/language/typescript.png"
					class="lang"
					alt="ts"
				/>
				Typescript
				<img
					src="/assets/language/mongodb.png"
					class="lang"
					alt="mongo"
				/>
				MongoDB
			</div>
			<a name="portfolio" />
			<br />
			<hr style="width: 90vw;" />
			<div class="projects MPageTxt">
				<h1>경력 & 프로젝트 Career & Projects</h1>
				<button class="collapsible tBlue tBold">경력 보기</button>
				<div class="CareerContent" style="text-align:center;">
					<div class="defaultCareer">
						<a class="tLime"> Hacking </a><br />
						<a
							>{#each data.career.hacking as cr, index}
								<span
									>{index + 1}. {cr}{index ===
									data.career.hacking.length - 1
										? ""
										: ""}</span
								><br />
							{/each}</a
						>
						<br />
						<a class="tRed"> Programming </a><br />
						<a
							>{#each data.career.programming as cr, index}
								<span
									>{index + 1}. {cr}{index ===
									data.career.programming.length - 1
										? ""
										: ""}</span
								><br />
							{/each}</a
						>
					</div>
				</div>
				<br /><br />
				<div class="projectDiv">
					<div class="whenPC">
						<p>
							&nbsp;<img
								align="center"
								src="https://github-readme-stats.vercel.app/api?username=ninejuan&show_icons=true&locale=en&theme=gotham"
								alt="ninejuan"
							/>
						</p>
					</div>
					<p>
						&nbsp;<img
							align="center"
							src="https://github-readme-stats.vercel.app/api/top-langs/?username=ninejuan&show_icons=true&locale=en&theme=gotham"
							alt="ninejuan"
						/>
					</p>
				</div>
			</div>
			<br />
		</section>
		<!-- Channel Plugin Scripts -->

		<!-- Channel Plugin Scripts -->
		<!-- Channel Plugin Scripts -->
		<script src="js/index.js"></script>
		<!-- End Channel Plugin -->
		<footer class="site-footer">
			<div class="container">
				<div class="row">
					<div class="col-sm-12 col-md-3">
						<h6 style="font-family: 'Jua', sans-serif;">정보</h6>
						<p class="text-justify" style="color: gray;">
							초보 화이트해커 주안입니다. 화이트햇 팀 <a
								href="https://secstf.kr"
								target="_blank"
								rel="noopener noreferrer"
								style="color:white;text-decoration:none;"
								>SnatchTheFlag</a
							>에서 활동하고 있습니다.
						</p>
					</div>

					<div class="col-sm-12 col-md-3">
						<h6 style="font-family: 'Jua', sans-serif;">개발</h6>
						<a>
							<img
								alt="Designed by JuanLee"
								src="/assets/profile.png"
								width="150"
								height="150"
							/>
						</a>
					</div>

					<div class="col-xs-6 col-md-3">
						<h6>주안Lab</h6>
						<ul class="footer-links">
							<li>
								<a
									href="https://306.juany.kr"
									target="_blank"
									rel="noopener noreferrer">아람이 대시보드</a
								>
							</li>
							<li>
								<a
									href="https://docs.aramy.net"
									target="_blank"
									rel="noopener noreferrer">아람이 API 문서</a
								>
							</li>
						</ul>
					</div>

					<div class="col-xs-6 col-md-3">
						<h6>Contact</h6>
						<ul class="footer-links">
							<li>
								<a href="mailto:{data.contact.mail}">Mail</a>
							</li>
							<li>
								<a
									href="https://github.com/{data.contact
										.github}"
									target="_blank"
									rel="noopener noreferrer">Github</a
								>
							</li>
							<li>
								<a
									href="https://discord.com/users/{data
										.contact.discord}"
									rel="noopener noreferrer">Discord</a
								>
							</li>
						</ul>
					</div>
				</div>
				<hr />
			</div>
			<div class="container">
				<div class="row">
					<div class="col-md-8 col-sm-6 col-xs-12">
						<p class="copyright-text">
							Copyright 2023 <a
								style="color: lime; text-decoration:none;"
								href="https://juany.kr"
								target="_blank"
								rel="noopener noreferrer">Juan Lee.</a
							> All Rights Reserved.
						</p>
					</div>
				</div>
			</div>
		</footer>
	</div></body
>
<slot />
<!-- 폰트 관련

더잠실체
KCC간판체 - 한저위-->
