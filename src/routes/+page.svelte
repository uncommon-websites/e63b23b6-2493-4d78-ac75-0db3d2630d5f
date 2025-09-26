<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
</script>

<Hero
	title="Test ideas. Skip the guesswork."
	subtitle="Validate new features with real user data."
	imageSrc="/generated/image-a-group-of-professional-product-managers.webp"
	centered={false}
/>
<LogoScroller 
	label="Trusted by industry leaders"
	logoUrls={[
		'https://cdn.brandfetch.io/slack.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/notion.so/w/400/h/400/logo',
		'https://cdn.brandfetch.io/figma.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/airtable.com/w/400/h/400/logo'
	]}
/>

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	testimonials={[
		{
			name: "Mei Chen",
			position: "Senior Product Manager",
			company: "DataFlow Technologies",
			quote:
				"We used to spend 3 weeks gathering user feedback through surveys and interviews. Now we validate features in 48 hours with real behavioral data. This saved us $40K in development costs on our last failed feature.",
			image: "/generated/image-professional-headshot-of-a-confident-asi.webp"
		},
		{
			name: "Marcus Williams",
			position: "Head of Product",
			company: "CloudScale Solutions",
			quote:
				"Before, 60% of our features flopped post-launch. The risk was killing our roadmap confidence. Now we de-risk every decision with actual user data, leading to an 85% feature success rate and faster product-market fit.",
			image: "/generated/image-professional-headshot-of-a-confident-bla.webp"
		},
		{
			name: "Isabella Rodriguez",
			position: "VP Product",
			company: "GrowthTech Inc",
			quote:
				"Our team was burning through $200K quarterly on features users didn't want. This platform cut our validation time from months to days, reducing our feature development costs by 70% while increasing user satisfaction.",
			image: "/generated/image-professional-headshot-of-a-confident-lat.webp"
		}
	]}
/>

<Features
	title="Validate faster, decide smarter"
	subtitle="Everything you need to test ideas with real users and ship features that matter"
	features={[
		{
			title: "Real-time user testing",
			description: "Get user feedback on prototypes and features within hours, not weeks. Skip the research agency bottleneck and validate ideas directly with your target audience."
		},
		{
			title: "AI-powered insight generation", 
			description: "Transform raw user feedback into actionable insights automatically. Our AI identifies patterns, prioritizes issues, and suggests improvements so you can focus on building."
		},
		{
			title: "Budget-friendly research plans",
			description: "Access professional-grade user research without the agency price tag. Scale your testing budget as you grow, starting at a fraction of traditional research costs."
		},
		{
			title: "Feature impact prediction",
			description: "Know which features will drive engagement before you build them. Our predictive models analyze user behavior to forecast feature success and ROI."
		},
		{
			title: "Scalable testing infrastructure",
			description: "Run multiple tests simultaneously without operational overhead. Our platform handles recruitment, scheduling, and data collection so your team can focus on product decisions."
		},
		{
			title: "Integrated analytics dashboard",
			description: "See all your user insights in one place with seamless integrations to your existing product analytics. Connect the dots between user feedback and product metrics effortlessly."
		}
	]}
/>
<AboutTeaser generating />
<CallToAction generating />
