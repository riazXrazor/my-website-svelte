<script>
	import Nav from '../components/Nav.svelte';
	import jQ from "jquery";

	export let segment;

	function handleLoad(){
			var isMobile = {
			Android: function() {
				return navigator.userAgent.match(/Android/i);
			},
				BlackBerry: function() {
				return navigator.userAgent.match(/BlackBerry/i);
			},
				iOS: function() {
				return navigator.userAgent.match(/iPhone|iPad|iPod/i);
			},
				Opera: function() {
				return navigator.userAgent.match(/Opera Mini/i);
			},
				Windows: function() {
				return navigator.userAgent.match(/IEMobile/i);
			},
				any: function() {
				return (isMobile.Android() || isMobile.BlackBerry() || isMobile.iOS() || isMobile.Opera() || isMobile.Windows());
			}
		};
		if ( !isMobile.any() ) {
			jQ('.js-fullheight').css('height', jQ(window).height());
			jQ(window).resize(function(){
				jQ('.js-fullheight').css('height', jQ(window).height());
			});
		}
	}
</script>

<style>
	main {
		/* position: relative; */
		/* max-width: 56em; */
		background-color: white;
		padding: 2em;
		margin: 0 auto;
		box-sizing: border-box;
	}
</style>

<div class="container-wrap">
<a href="/" class="js-colorlib-nav-toggle colorlib-nav-toggle" data-toggle="collapse" data-target="#navbar" aria-expanded="false" aria-controls="navbar"><i></i></a>
	<Nav {segment}/>

	<main id="colorlib-main">
		<slot></slot>
	</main>
</div>

<svelte:window on:load={handleLoad}/>
