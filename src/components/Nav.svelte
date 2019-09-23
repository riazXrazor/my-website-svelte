<script>
	export let segment;
</script>

<aside id="colorlib-aside" role="complementary" class="border js-fullheight">
			<div class="text-center">
				<div class="author-img" style="background-image: url(images/about.jpg);"></div>
				<h1 id="colorlib-logo"><a href="index.html">Riaz Laskar</a></h1>
				<span class="position"><a href="/">UI Engineer</a> in India</span>
			</div>
			<nav id="colorlib-main-menu" role="navigation" class="navbar">
				<div id="navbar" class="collapse">
					<ul>
						<li class="{ segment == undefined ? 'active' : '' }"><a href="/" data-nav-section="home">Home</a></li>
						<li class="{ segment == 'about' ? 'active' : '' }" ><a href="about" data-nav-section="about">About</a></li>
						<li class="{ segment == 'services' ? 'active' : '' }" ><a href="services" data-nav-section="services">Services</a></li>
						<li class="{ segment == 'skills' ? 'active' : '' }" ><a href="skills" data-nav-section="skills">Skills</a></li>
						<li class="{ segment == 'education' ? 'active' : '' }" ><a href="education" data-nav-section="education">Education</a></li>
						<li class="{ segment == 'experience' ? 'active' : '' }" ><a href="experience" data-nav-section="experience">Experience</a></li>
						<li class="{ segment == 'work' ? 'active' : '' }" ><a href="work" data-nav-section="work">Work</a></li>
						<li class="{ segment == 'contact' ? 'active' : '' }" ><a href="contact" data-nav-section="contact">Contact</a></li>
					</ul>
				</div>
			</nav>

			<div class="colorlib-footer">
				<p><small>Copyright &copy; {new Date().getFullYear()} All rights reserved </small></p>
				<ul>
					<li><a href="/"><i class="icon-facebook2"></i></a></li>
					<li><a href="/"><i class="icon-twitter2"></i></a></li>
					<li><a href="/"><i class="icon-instagram"></i></a></li>
					<li><a href="/"><i class="icon-linkedin2"></i></a></li>
				</ul>
			</div>

		</aside>