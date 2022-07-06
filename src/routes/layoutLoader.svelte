<script lang="ts">
	import { navigating } from '$app/stores';

	import { loading } from '$lib/loading';
	import Loading from '$lib/Loading.svelte';

	$: loading.setNavigate(!!$navigating);
</script>

<slot />

<button on:click={() => loading.setLoading(true, "I'm loading")}>Set Loading</button>
<button on:click={() => loading.setLoading(false)}>Stop Loading</button>

<Loading />
