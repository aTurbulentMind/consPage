<body>
	<h1>Gallery</h1>

	<h2>A: like a grid of pictures</h2>

	<div class="container" style="margin-bottom:25%;">
		<div class="box a"><img src="img/purp.png" alt="" /></div>
		<div class="box b"><img src="img/purp.png" alt="" /></div>
		<div class="box c"><img src="img/purp.png" alt="" /></div>
		<div class="box d"><img src="img/purp.png" alt="" /></div>
		<div class="box e"><img src="img/purp.png" alt="" /></div>
		<div class="box f"><img src="img/purp.png" alt="" /></div>
		<div class="box g"><img src="img/purp.png" alt="" /></div>
		<div class="box h"><img src="img/purp.png" alt="" /></div>
		<div class="box i"><img src="img/purp.png" alt="" /></div>
		<div class="box j"><img src="img/purp.png" alt="" /></div>
	</div>

	<h2>B: like a slide show that scrolls sideways</h2>

	<div class="media-scroller snaps-inline" style="margin-bottom:15% ;">
		<div class="media-element"><img src="/img/purp.png" alt="" /></div>
		<div class="media-element"><img src="/img/purp.png" alt="" /></div>
		<div class="media-element"><img src="/img/purp.png" alt="" /></div>
		<div class="media-element"><img src="/img/purp.png" alt="" /></div>
		<div class="media-element"><img src="/img/purp.png" alt="" /></div>
		<div class="media-element"><img src="/img/purp.png" alt="" /></div>
		<div class="media-element"><img src="/img/purp.png" alt="" /></div>
		<div class="media-element"><img src="/img/purp.png" alt="" /></div>
		<div class="media-element"><img src="/img/purp.png" alt="" /></div>
		<div class="media-element"><img src="/img/purp.png" alt="" /></div>
		<div class="media-element"><img src="/img/purp.png" alt="" /></div>
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
