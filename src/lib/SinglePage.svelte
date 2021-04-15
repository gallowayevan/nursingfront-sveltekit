<script>
	export let title = 'Title';
</script>

<section class="section columns is-centered">
	<article class="content column is-half">
		<h1 class="title is-spaced has-text-weight-light">{title}</h1>
		<slot />
	</article>
</section>
