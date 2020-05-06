<template>
  <div id="app">

    <header class="header">
      <div class="header__left">
				<g-link to='/'><img id='ryu' src='../assets/images/ryu.jpg' /></g-link>
				<!-- Layout Default.vue -->
      </div>

      <div class="header__right">
        <ToggleTheme />
      </div>
    </header>

		<nav id='navbar'>
			<g-link class='nav-link' to='/'>blog</g-link>
			<g-link class='nav-link' to='/about'>about</g-link>
			<g-link class='nav-link' to='/contact'>contact</g-link>
		</nav>

    <main class="main">
      <slot/>
    </main>

    <footer class="myfooter">
      <p><span class="footer__copyright">Copyright &copy; {{ new Date().getFullYear() }} | RyuCave.com</span></p>
      <p><span class="footer__links">Created by <a href="https://simonhlee97.github.io/" target="_blank">Simon Lee</a></span></p>
			<p>powered by: <a href="https://gridsome.org/" target="_blank">Gridsome</a> and <a href="https://netlifycms.org/" target="_blank">NetlifyCMS</a></p>
    </footer>

  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import ToggleTheme from '~/components/ToggleTheme.vue'

export default {
  props: {
    showLogo: { default: true }
  },
  components: {
    Logo,
    ToggleTheme
  }
}
</script>

<style lang="scss">
.myfooter {
	width: 100%;
	line-height: 11px;
	height: 30vh;
	// background-color: black;
	padding: calc(var(--space) / 2);
  text-align: center;
	font-size: .8em;
	> span {
    margin: 0 .35em;
  }

  a {
    color: currentColor;
  }
}
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  min-height: var(--header-height);
  padding: 0 calc(var(--space) / 2);
  top:0;
  z-index: 10;

  &__left,
  &__right {
    display: flex;
    align-items: center;
  }

  @media screen and (min-width: 1300px) {
    //Make header sticky for large screens
    position: sticky;
    width: 100%;
  }
}

.main {
  margin: 0 auto;
  padding: 1.5vw 15px 0;
}

#ryu {
	width: 80px;
	height: auto;
	border-radius: 40%;
	margin-top: 10px;
}

#navbar {
	text-align: center;
}
.nav-link {
	font-size: 0.7rem;
	margin: 8px;
	text-transform: uppercase;
	text-decoration-line: none;
}
.nav-link:hover {
	text-decoration-line: underline;
}
</style>
