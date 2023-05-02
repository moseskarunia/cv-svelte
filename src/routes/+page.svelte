<div class="readable-area">
	<a class="header" href="./photo.html">
		<div class="header-text">
			<h1>Squarepants, Spongebob</h1>
			<p>Head Chef</p>
		</div>
		<img
			alt="spongebob avatar"
			class="avatar"
			src="https://play-lh.googleusercontent.com/9XA4q4TKYtF2l5oN10M8oumPauR9g5lFOAJXjczrd3Gmq9cwQ8QOQJ-2KZv84s1oTA"
		/>
	</a>

	<div class="content">
		<div class="content-column">
			<div class="section-title">
				<i class="fa fa-solid fa-user" />
				Profile
			</div>
			<br />
			<p>
				Hello, my name is Spongebob Squarepants and I'm passionate about creating the best possible
				food. In my spare time, I like to catch jellyfishes with my trusty net.
			</p>
			<br />
			<div class="section-title">
				<i class="fa fa-solid fa-book" />
				Education
			</div>
			<br />
			<ul>
				<li>
					2011-2014
					<br />
					&emsp; Bikini Bottom High School
				</li>
				<li>
					2014-2018
					<br />
					&emsp; New Kelp City Culinary College
				</li>
			</ul>
		</div>
		<div class="content-column">
			<div class="section-title">
				<i class="fa fa-solid fa-briefcase" />
				Work History
			</div>
			<br />
			<ul>
				<li>
					Head Cook (2022 - ongoing)
					<br />
					&emsp; Krusty Krab, Inc.
				</li>
				<li>
					Marketing Associate (2020 - 2022)
					<br />
					&emsp; Chum Bucket Ltd.
				</li>
				<li>
					Jellyfish Catcher (2018 - 2020)
					<br />
					&emsp; Freelance
				</li>
			</ul>
			<br />
			<div class="section-title">
				<i class="fa fa-solid fa-wand-sparkles" />
				Skills
			</div>
			<br />
			<ul>
				<li>
					<span>Jellyfish Hunting</span>
					<div class="gauge">
						<div class="bullet filled-bullet" />
						<div class="bullet filled-bullet" />
						<div class="bullet filled-bullet" />
						<div class="bullet filled-bullet" />
						<div class="bullet filled-bullet" />
					</div>
				</li>
				<li>
					<span>English</span>
					<div class="gauge">
						<div class="bullet filled-bullet" />
						<div class="bullet filled-bullet" />
						<div class="bullet filled-bullet" />
						<div class="bullet filled-bullet" />
						<div class="bullet" />
					</div>
				</li>
				<li>
					<span>Whale Singing</span>
					<div class="gauge">
						<div class="bullet filled-bullet" />
						<div class="bullet filled-bullet" />
						<div class="bullet filled-bullet" />
						<div class="bullet" />
						<div class="bullet" />
					</div>
				</li>
			</ul>
		</div>
	</div>
</div>

<style>
	h1 {
		font-family: 'peralta';
	}

	ul {
		list-style-type: none;
	}

	li {
		display: flex;
		flex-direction: row;
		align-items: center;
		justify-content: space-between;
	}

	li span {
		margin-right: 16px;
	}

	.gauge {
		display: flex;
		flex-direction: row;
	}

	.bullet {
		border-radius: 100%;
		width: 16px;
		height: 16px;
		margin: 4px;
		background-color: #fff59d;
	}

	.filled-bullet {
		background-color: #fbc02d;
	}

	.header-text {
		text-align: end;
		flex: 1;
		margin-right: 16px;
	}

	.readable-area {
		display: flex;
		flex-direction: column;
		background-color: #ffffff;
		margin: 0 15%;
	}

	.header {
		padding: 16px;
		display: flex;
		flex: row;
		align-items: center;
		border-bottom: 2px solid black;
		text-decoration: none;
		color: #000000;
	}

	.content {
		display: flex;
		flex-direction: row;
	}

	.content-column {
		flex: 1;
		margin-top: 16px;
		padding: 0 16px 16px 16px;
		background-color: #ffffff;
	}

	img {
		width: 128px;
		height: 128px;
		border: 4px solid #000000;
		border-radius: 100%;
	}

	.fa.fa-solid {
		margin-right: 8px;
	}

	.section-title {
		background-color: #ffeb3b;
		border-left: 4px solid #fbc02d;
		color: black;
		padding: 8px 16px;
		text-transform: UPPERCASE;
		font-weight: 500;
	}

	i {
		background-color: transparent;
	}

	@media (max-width: 600px) {
		.header {
			flex-direction: column-reverse;
		}

		.header-text {
			text-align: center;
		}

		.content {
			flex-direction: column;
		}
	}
</style>
