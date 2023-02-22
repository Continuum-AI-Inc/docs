<script lang="ts">
	import Button from "./Button.svelte";
	export let link: string;
</script>

<Button {link} type="github"><slot></slot></Button>