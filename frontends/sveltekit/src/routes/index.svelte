<script lang='ts' context='module'>
import { browser } from "$app/env";


    export async function  load() {
        const response = await (await fetch(browser ? 'http://localhost:3000/api/test' : 'http://api:8080/api/test')).text();
		return {
			props: {
				apiResponse: response
			}
		};
	}
</script>

<script>
    export let apiResponse = ''
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
<p>This is the Response from API: <strong>{apiResponse}</strong></p>
