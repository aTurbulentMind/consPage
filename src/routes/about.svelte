<script context="module">
	function sleep(ms) {
		return new Promise((resolve) => setTimeout(resolve, ms));
	}

	export async function load() {
		await sleep(2000);

		return {
			status: 200
		};
	}
</script>

<h1>About</h1>
<a href="/">Home</a>
