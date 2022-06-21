<style>
	@import url("https://unpkg.com/fluent-svelte/theme.css");
	:global(body) {
		background-color: var(--fds-solid-background-base);
		color: var(--fds-text-primary);
	}
</style>

<script>
	import { TextBox } from "fluent-svelte";
	import GradientText from 'svelte-gradient-typography';
	let value = "";
</script>

<TextBox placeholder="Chose a Name" bind:value />

<GradientText>
    The {value}
</GradientText>
