
<script>
	import  ServiceCard  from '../components/ServiceCard.svelte'
	import  PageHead  from '../components/PageHead.svelte'
	const services = [
		{
			icon: 'bulb',
			color: 'color-1',
			title: 'Innovative Ideas',
			description: 'Separated they live in Bookmarksgrove right at the coast of the Semantics' 
		},
		{
			icon: 'bulb',
			color: 'color-2',
			title: 'Innovative Ideas',
			description: 'Separated they live in Bookmarksgrove right at the coast of the Semantics' 
		},
		{
			icon: 'bulb',
			color: 'color-3',
			title: 'Innovative Ideas',
			description: 'Separated they live in Bookmarksgrove right at the coast of the Semantics' 
		},
		{
			icon: 'layers2',
			color: 'color-4',
			title: 'Graphic Design',
			description: 'Separated they live in Bookmarksgrove right at the coast of the Semantics' 
		},
		{
			icon: 'data',
			color: 'color-5',
			title: 'Software',
			description: 'Separated they live in Bookmarksgrove right at the coast of the Semantics' 
		},
		{
			icon: 'phone3',
			color: 'color-6',
			title: 'Application',
			description: 'Separated they live in Bookmarksgrove right at the coast of the Semantics' 
		},
	];
</script>
					<div class="row">
						<PageHead subheading="HERE ARE SOME OF MY" heading="WHAT I DO?" />
					</div>
					<div class="row row-pt-md">
						{#each services as service}
							<div class="col-md-4 text-center">
								<ServiceCard {...service} />
							</div>
						{/each}
					</div>
