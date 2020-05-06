<template>
	<div class="author">
		<h1 v-if="showTitle" class="author__site-title">
			{{ $static.metadata.siteName }}.com
		</h1>

		<p class="author__intro">
			Hadouken! Welcome to Simon's online cave.
		</p>

		<p class="author__links">
			
			
			<a href="https://twitter.com/simonhlee97"><font-awesome :icon="['fab', 'twitter']"/></a>
			<a href="https://github.com/simonhlee97"><font-awesome :icon="['fab', 'github']"/></a>
		</p>

	</div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
export default {
	props: ['showTitle']
}
</script>

<style lang="scss">
.author {
	margin: 0 auto;
	max-width: 500px;
	text-align: center;
	padding-bottom: calc(var(--space) / 2);

	&__image {
		border-radius: 100%;
		width: 90px;
		height: 90px;
		margin-bottom: 1em;
	}

	&__intro {
		opacity: .8;
	}

	&__site-title {
		margin: 0 auto;
		font-size: 2rem;
		text-transform: uppercase;
		letter-spacing: 5px;
		max-width: 400px;
	}

	&__links {
		margin-top: -.5em;
		a {
			margin: 0 .5em;
		}
	}
}
</style>
