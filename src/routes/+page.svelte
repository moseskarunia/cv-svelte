<script lang="ts">
	import Section from '$components/Section.svelte';
	import book from 'svelte-awesome/icons/book';
	import briefcase from 'svelte-awesome/icons/briefcase';
	import cogs from 'svelte-awesome/icons/cogs';
	import user from 'svelte-awesome/icons/user';
</script>

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
		<Section iconData={user} title="Profile">
			<p>
				Hello, my name is Spongebob Squarepants and I'm passionate about creating the best possible
				food. In my spare time, I like to catch jellyfishes with my trusty net.
			</p>
		</Section>
		<Section iconData={book} title="Education">
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
		</Section>
		<Section iconData={briefcase} title="Work History">
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
		</Section>
		<Section iconData={cogs} title="Skills">
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
		</Section>
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
		text-align: center;
		flex: 1;
		margin-right: 16px;
	}

	.readable-area {
		display: flex;
		flex-direction: column;
		background-color: #ffffff;
		margin: 0 5%;
		height: 100%;
	}

	.header {
		padding: 16px;
		display: flex;
		flex-direction: column-reverse;
		align-items: center;
		border-bottom: 2px solid black;
		text-decoration: none;
		color: #000000;
	}

	.content {
		display: grid;
		grid-template-columns: repeat(1, minmax(0, 1fr));
		gap: 32px;
		padding: 32px 32px;
	}

	img {
		width: 128px;
		height: 128px;
		border: 4px solid #000000;
		border-radius: 100%;
	}

	@media (min-width: 600px) {
		.header {
			flex-direction: row;
		}

		.header-text {
			text-align: end;
		}

		.content {
			grid-template-columns: repeat(2, minmax(0, 1fr));
		}

		.readable-area {
			margin: 0 10%;
		}
	}

	@media (min-width: 1000px) {
		.readable-area {
			margin: 0 20%;
		}
	}
</style>
