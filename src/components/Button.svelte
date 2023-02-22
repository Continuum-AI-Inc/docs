<script lang="ts">
	export let icon: string = "";
	export let type: "github" | "default" = "default";
	export let link: string;
</script>

<a class="button {type}" href={link}>
	{#if type == "github"}
		<img src="/icons/github-mark-white.svg" alt="GitHub" width=20>
	{:else if icon}
		<span class="material-symbols-outlined">{icon}</span>
	{/if}
<slot></slot>
</a>

<style lang="scss">
	a.button {
		background-color: #3A86FF;
		color: #fafafa;
		border-radius: 8px;
		padding: 16px;
		display: flex;
		text-decoration: none;
		align-items: center;
		justify-content: center;
		gap: 8px;
		font-size: 18px;
		font-weight: 600;
		border: none;
		cursor: pointer;
		box-shadow: 1px 1px 4px 0px rgba(0,0,0,0.3);
		transition: background-color 0.4s ease;

		&:hover {
			background-color: darken(#3A86FF, 15);
		}
	}

	a.button.github {
		background-color: #333;

		&:hover {
			background-color: lighten(#333, 10);
		}
	}
</style>