<body>
	<h1>Merch</h1>

	<p>
		Go buy shit from my store by clicking this button
		<br />
		<a href="https://www.storefrontier.com/concrete/">Buy now!</a>
	</p>

	<h1>Gallery</h1>

	<div class="container" style="margin-bottom:25%;">
		<div class="box a"><img src="img/gallow/one.jpeg" alt="" /></div>
		<div class="box b"><img src="img/gallow/two.jpeg" alt="" /></div>
		<div class="box c"><img src="img/gallow/three.jpeg" alt="" /></div>
		<div class="box d"><img src="img/gallow/four.jpeg" alt="" /></div>
		<div class="box e"><img src="img/gallow/five.jpeg" alt="" /></div>
		<div class="box f"><img src="img/gallow/six.jpeg" alt="" /></div>
		<div class="box g"><img src="img/gallow/seven.jpeg" alt="" /></div>
		<div class="box h"><img src="img/gallow/eight.jpeg" alt="" /></div>
		<div class="box i"><img src="img/gallow/nine.jpeg" alt="" /></div>
		<div class="box j"><img src="img/gallow/ten.jpeg" alt="" /></div>
	</div>
</body>

<style lang="scss">
	@import 'styles/components';

	.box {
		border: 1px solid #ccc;
	}

	img {
		width: 100%;
	}

	.media-scroller {
		border: 1px solid #ccc;
		--spacer: 2rem;
		display: grid;
		grid-auto-flow: column;
		grid-auto-columns: 100%;
		padding: var(--spacer);
		gap: 7%;
		margin: 2%;
		overflow-x: auto;
		overscroll-behavior-inline: contain;
	}

	.media-element {
		display: grid;
		padding: 3%;
		background-color: $backgroundSecond;
		border-radius: 3px;
		box-shadow: $shade;

		img {
			inline-size: 100%;
			object-fit: cover;
		}
	}

	.snaps-inline {
		scroll-snap-type: inline mandatory;
		scroll-padding-inline: var(--spacer);

		* {
			scroll-snap-align: start;
		}
	}
</style>
