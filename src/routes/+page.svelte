<script>
	import { TextBox, Button, TextBlock } from 'fluent-svelte';
	import 'fluent-svelte/theme.css';

	let count = 0;
</script>

<style>
	/* Some base styles to get things looking right. */
	:global(body) {
		background-color: var(--fds-solid-background-base);
		color: var(--fds-text-primary);
	}
</style>

<div>
	<form>
		<h3>Reference a website</h3>
		<p>Our tool will automatically query the site for it's data and it'll fill in the values below, if any are left empty it means the tool failed to find those types of data and you should enter them manually.</p>

		<TextBox placeholder="Enter the site URL" />
		<Button>Query data</Button>
	</form>
</div>
