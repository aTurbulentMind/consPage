<body>
	<h1>Upcoming Shows</h1>
	<background>
		<a href="https://www.brownpapertickets.com/event/5410347/">
			<tour>SO North West 7-9-2022</tour>
			<img src="/img/flyerTwo.jpg" alt="" />
		</a>
	</background>

	<background>
		<a href="https://www.brownpapertickets.com/event/5469054/">
			<tour>Wicked Warlords 7-14-2022</tour>
			<img src="/img/baintA.jpg" alt="" />
		</a>
	</background>
</body>

<style lang="scss">
	@import 'styles/components';

	background {
		tour {
			margin: -7% 12%;
			font-size: 4vw;
			font-weight: 600;
		}
	}
	img {
		width: 65%;
		height: 65%;
		margin: 15%;
		overflow-x: hidden;
		@include glassBack;

		&:hover {
			transition: $transitSpeed ease-in-out;
			width: 85%;
			height: 85%;
			margin: 5%;
			box-shadow: 0 3px 12px 15px $backgroundSecond;
		}
	}

	@media only screen and (min-width: 770px) {
		img {
			width: 40%;
			height: 40%;
			margin: 10% 20%;

			&:hover {
				width: 40%;
				height: 40%;
				margin: 10% 20%;
			}
		}
	}
</style>
