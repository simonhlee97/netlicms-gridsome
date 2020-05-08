<template>
  <Layout :show-logo="true">
    
		<div class="about">
			
			<h1 class='text-center'>About RyuCave.com</h1>
			<p>This is a blog I created during the Big COVID-19 Quarantine. I'm going to write about whatever is on my mind, so no limit to the number of topics. However, I do all my web-dev-related writing at <a href="https://dev.to/simonhlee97">Dev.to</a>.</p>
			<h4>RyuCave Toolbox:</h4>
			<ul>
					<li>MacBook Air</li>
					<li>Static site generator: <a href='https://gridsome.org'>Gridsome</a></li>
					<li>CMS: <a href='https://netlifycms.org'>NetlifyCMS</a></li>
					<li>Hosting: <a href='https://netlify.com'>Netlify</a></li>
					<li>Editor: <a href='https://code.visualstudio.com'>VS Code</a></li>
			</ul>

			<hr id='about-line' class='text-center'>

			<h1 class='text-center'>About Me</h1>

			<section>
				<h4>I'm Simon.</h4>
				<p>Born in Korea, and grew up in Hoosier country (Indiana).</p>
				<p>I'm basically a redneck from Indiana trapped in a Korean man's body.</p>
				<p>I love basketball (Pacers), tennis, reading, coding, photography, tacos, pizza, and coffee.</p>
				<p>As of now (May 2020) I'm currently stuck in South Korea due to COVID-19 (which is probably a good thing). Most likely, I will be moving back to the US in a year or 2.</p>
			</section>

			<section>
				<h4>Some of my favorite Podcasts, Blogs, etc.</h4>
				<ul>
					<li><a href='https://samharris.org'>Sam Harris</a></li>
					<li><a href='https://freakonomics.com'>Freakonomics</a></li>
					<li><a href='https://danpink.com'>Dan Pink</a></li>
					<li><a href='https://ma.tt'>Matt Mullenweg</a></li>
					<li><a href='https://marginalrevolution.com'>Marginal Revolution</a></li>
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