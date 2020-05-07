<template>
  <Layout :show-logo="true">
    
		<div class="about">
			
			<h1 class='text-center'>About RyuCave.com</h1>
			<p>This is a blog I created during the Big COVID-19 Quarantine. I'm going to write about whatever is on my mind, so no limit to the number of topics. However, I do all my web-dev-related writing at <a href="https://dev.to/simonhlee97">Dev.to</a>.</p>
			<h3>My Toolbox:</h3>
			<ul>
					<li>MacBook Air (2016?)</li>
					<li>Static site generator: Gridsome</li>
					<li>CMS: NetlifyCMS</li>
					<li>Hosting: Netlify</li>
					<li>Editor: VS Code</li>
			</ul>

			<hr id='about-line' class='text-center'>

			<h1 class='text-center'>About Me</h1>

			<section>
				<h3>I'm Simon.</h3>
				<p>Born in Korea, and grew up in Hoosier country (Indiana).</p>
				<p>I'm basically a redneck from Indiana trapped in a Korean man's body.</p>
				<p>I love basketball (Pacers), tennis, reading, coding, photography, tacos, pizza, and coffee.</p>
				<p>As of now (May 2020) I'm currently stuck in South Korea due to COVID-19 (which is probably a good thing). Most likely, I will be moving back to the US in a year or 2.</p>
			</section>

			<section>
				<h3>My Favorite Podcasts, Blogs, and Websites (non-tech)</h3>
				<ul>
					<li>Sam Harris</li>
					<li>Freakonomics</li>
					<li>Dan Pink</li>
					<li>Matt</li>
					<li>Marginal Revolution</li>
				</ul>
			</section>

		</div>

  </Layout>
</template>

<style lang='scss' scoped>
	.about {
		padding: 2em 6.5em;
	}
	ul {
		line-height: 16px;
	}
	#about-line {
		margin: 5em 0;
	}

</style>