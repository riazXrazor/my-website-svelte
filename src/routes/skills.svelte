<script>
	import  PageHead  from '../components/PageHead.svelte'
	import  SkillBar  from '../components/SkillBar.svelte'
	const skills = [
		{
			name: 'Javascript',
			percent: 80,
			color: 'color-1'
		},
		{
			name: 'React',
			percent: 65,
			color: 'color-2'
		},
		{
			name: 'Vue',
			percent: 60,
			color: 'color-3'
		},
		{
			name: 'PHP',
			percent: 60,
			color: 'color-4'
		},
		{
			name: 'Mysql',
			percent: 50,
			color: 'color-5'
		},
		{
			name: 'Laravel',
			percent: 75,
			color: 'color-6'
		},
		{
			name: 'Node.Js',
			percent: 70,
			color: 'color-6'
		},
	]
</script>
					<div class="row">
						<PageHead heading="My Specialty" subheading="My Skills" />
					</div>
					<div class="row">
						<div class="col-md-12" data-animate-effect="fadeInLeft">
							<p>The Big Oxmox advised her not to do so, because there were thousands of bad Commas, wild Question Marks and devious Semikoli, but the Little Blind Text didn’t listen. She packed her seven versalia, put her initial into the belt and made herself on the way.</p>
						</div>
						{#each skills as skill}
							<div class="col-md-6">
								<SkillBar {...skill} />
							</div>
						{/each}
					</div>
