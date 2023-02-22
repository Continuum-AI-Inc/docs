<div class="warn">
	<h4>Warning!</h4>
	<slot></slot>
</div>

<style lang="scss">
	.warn {
		border-left: 4px solid #ffb238;
		background-color: rgba(255, 178, 56, 0.2);
		padding: 15px 24px;
		font-size: 18px;
		font-weight: 500;
		border-radius: 4px;
	}

	h4 {
		font-size: 18px;
		margin: 0;
		margin-bottom: 8px;
	}
</style>