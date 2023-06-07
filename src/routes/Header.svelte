<script>
  import { page } from '$app/stores';
	import { writable } from 'svelte/store';

  let currentPage = writable(''); 
	let pageDescription =writable('');

  $: {
    // Get the current page URL pathname from the $page store
    const currentPath = $page.url.pathname;

    // Update the currentPage variable based on the current path
    if (currentPath === '/') {
      currentPage.set('Welcome');
			pageDescription.set('')
    } else if (currentPath === '/zipDomains') {
      currentPage.set('Zip Domains');
			pageDescription.set('Zip Domains are a malicious trick that can lead to individuals devulging valuable information all because they thought they where downloading a file')
    } else if (currentPath.startsWith('/WebSkimmers')) {
      currentPage.set('Web Skimmers');
			pageDescription.set('Web Skimmers attacking popular ecommerce sites is more common now than ever and can lead to your sensitive information being at risk')
    } else {
      currentPage.set('Unknown Page');
    }
  }
</script>

<header>
	<div class="header-content">
		<div class="header-left">
			<h1 class="page-title">{$currentPage}</h1>
			<p class="page-description">{$pageDescription}</p>
		</div>
		<nav class="header-right">
			<ul>
				<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
					<a href="/">Home</a>
				</li>
				<li aria-current={$page.url.pathname === '/zipDomains' ? 'page' : undefined}>
					<a href="/zipDomains">Zip Domains</a>
				</li>
				<li aria-current={$page.url.pathname.startsWith('/WebSkimmers') ? 'page' : undefined}>
					<a href="/WebSkimmers">Web Skimmers</a>
				</li>
			</ul>
		</nav>
	</div>
</header>

<style>
header {
	background-color: #E4EFEC;
	padding: 10px;
}

.header-content {
	display: flex;
	flex-direction:flex-start;
	justify-content: space-between;
	align-items: left;
}

.page-title {
	margin: 0;
	font-size: 3rem;
	font-weight: bold;
	position:relative;
	justify-self:left;
	margin-right:auto;
}

.page-description {
	margin: 0;
	font-size: 1rem;
	font-weight:lighter;
	inline-size: 20rem;
  overflow-wrap: break-word;
}

.header-left {
	display: flex;
	flex-direction: column;
}

.header-right {
	display: flex;
}

nav ul {
	list-style: none;
	padding: 0;
	margin: 0;
	display: flex;
	justify-content: center;
	align-items: center;
}

nav li {
	margin: 0 10px;
}

nav li[aria-current='page'] a {
	background-color: var(--button-color-primary);
	color: var(--button-color-secondary);
}

nav a {
	display: inline-block;
	padding: 10px 20px;
	border: 1px solid #333;
	border-radius: 10px;
	text-decoration: none;
	color: var(--color-accent);
	font-weight: 700;
	font-size: 0.8rem;
	text-transform: uppercase;
	letter-spacing: 0.1em;
	transition: color 0.2s linear;
}

a:hover {
	color: var(--color-accent);
}
</style>
