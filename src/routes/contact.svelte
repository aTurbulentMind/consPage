<body>
	<h1>Contact Us</h1>

	<div class="social">
		<h2>You can find me on Facebook</h2>
		<a href="https://www.facebook.com/harboreddreams"> <img src="img/purp.png" alt="" /></a>
	</div>

	<div class="social">
		<h2>Or follow me on Twitter</h2>
		<a href="https://twitter.com/CON_CRETE/"> <img src="img/purp.png" alt="" /></a>
	</div>
</body>

<style lang="scss">
	@import 'styles/components';

	.resizedTextbox {
		width: 300px;
		height: 50px;
	}

	.form {
		@include glassBack();
		margin: 0 13% 25% 13%;
		padding: 10%;
		contain: content;
	}

	h2 {
		margin-bottom: 10%;
	}

	h3 {
		font-weight: 100;
		font-size: 3.5vw;
		margin-bottom: 15%;
	}

	p {
		margin: 7% 0;
	}

	button {
		background: rgba(16, 15, 17, 0.616);
		outline: none;
		font-weight: 100;
		letter-spacing: 2px;
		border: 1px solid white;
		color: $textColorMain;
		text-transform: uppercase;
		padding: 10px;
		margin: 15% 0 10% 0;

		&:hover {
			transition: all 0.2s ease-in-out;
			background: $textColorMain;
			color: $backgroundMain;
			transform: scale(1.05);
		}
	}

	img {
		width: 90%;
		height: 90%;
		margin: 4% 4% 20% 4%;
		border: 1px solid $backgroundSecond;
		border-radius: 2%;
	}

	@media (min-width: 750px) {
		img {
			width: 85%;
			margin: 4% 0 10% 10%;
		}
	}
</style>
