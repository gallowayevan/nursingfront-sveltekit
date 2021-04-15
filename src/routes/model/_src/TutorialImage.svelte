<script>
	export let imageFileName;
</script>

<div>
	<slot />
	<img class="image" alt="Chart tutorial." src="/images/model/tutorial/{imageFileName}" />
	<hr />
</div>
