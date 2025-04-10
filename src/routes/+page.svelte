<script>
	let count = $state(4);
	setInterval(() => {
		if (count > 1) {
			count -= 1;
		}
	}, 950);
	$effect(() => {
		if (count === 1) {
			// window.location.href = 'https://getwronged.com';
		}
	});
</script>

<main>
	<h1>Wronged has moved</h1>
	<p>
		Redirecting you to <a href="https://getwronged.com">getwronged.com</a> in {count}.
	</p>
	<p>Relogin to continue where you left off.</p>
</main>

<style>
	main {
		min-height: 100dvh;
		text-align: center;
		background-color: #fff7ed;
		display: grid;
		justify-content: center;
		align-content: center;
	}
	/* playfair-display-latin-600-normal */
	@font-face {
		font-family: 'Playfair Display';
		font-style: normal;
		font-display: swap;
		font-weight: 600;
		src:
			url(@fontsource/playfair-display/files/playfair-display-latin-600-normal.woff2)
				format('woff2'),
			url(@fontsource/playfair-display/files/playfair-display-latin-600-normal.woff) format('woff');
		unicode-range:
			U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329,
			U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
	}
	/* montserrat-latin-400-normal */
	@font-face {
		font-family: 'Montserrat';
		font-style: normal;
		font-display: swap;
		font-weight: 400;
		src:
			url(@fontsource/montserrat/files/montserrat-latin-400-normal.woff2) format('woff2'),
			url(@fontsource/montserrat/files/montserrat-latin-400-normal.woff) format('woff');
		unicode-range:
			U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329,
			U+2000-206F, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
	}
	h1 {
		font-family: 'Playfair Display Variable', serif;
		font-weight: 600;
		font-size: 7rem;
		color: rgba(0, 0, 0, 0.8);
	}
	p {
		font-family: 'Montserrat', sans-serif;
		display: inline-block;
		color: #7c2808;
		margin-bottom: 0.5rem;
	}
	a {
		color: #531b06;
		text-decoration: underline;
		text-decoration-skip-ink: none;
		text-underline-offset: 3px;
		text-decoration-thickness: 2px;
	}
</style>
