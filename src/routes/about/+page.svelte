<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Innovation",
			description: "Constantly challenging the status quo to create better solutions."
		},
		{
			title: "Integrity",
			description: "Building trust through transparent actions and honest communication."
		},
		{
			title: "Impact",
			description: "Measuring our success by the positive change we create for our clients."
		}
	];
</script>

<SecondaryHero
	title="Real answers, fast"
	subtitle="User insights, without the wait"
	imageSrc="/generated/image-a-group-of-diverse-professionals-gathere.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Series A product managers are under constant pressure to move quickly. Growth targets don't wait—but traditional user research does. Weeks to schedule interviews, thousands spent on panels, and results that often contradict each other. Our founders had been there themselves—launching products, chasing signals, and making decisions with more gut than data. The gap between the speed of building and the slowness of research was costing teams time, budget, and clarity.",
		"Jorge Dobón, Mario Navarro, Julio Ribes, and Álvaro Callejo came together to solve the problem they deeply understood. With backgrounds spanning product, venture, and startups, they knew firsthand the cost of moving fast without real insight. Their solution? A new kind of research tool built for product managers—where recruiting users is instant, feedback is fast, and insights are clear. Inspired by tools like Notion and Figma, they designed a platform that brings research closer to where decisions happen: inside fast-moving product teams.",
		"Today, we help product teams validate features in days, not weeks. What once took piles of spreadsheets and lengthy processes now takes a few clicks. With real users and real data from the start, teams reduce the risk of building things no one needs. Our mission is simple—help every product decision feel confident, not hopeful. Because when you stop guessing and start listening, what you build gets better."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} generating />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	generating
	stakeholderType="team"
	title="Our team."
	subtitle="Your partners in innovation."
	stakeholders={[
		{
			name: "Alex Morgan",
			position: "Founder & CEO",
			bio: "Started the company with a vision to transform the industry through innovative solutions.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Jamie Chen",
			position: "Chief Design Officer",
			bio: "Award-winning designer with a passion for creating intuitive and beautiful experiences.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Taylor Wright",
			position: "Head of Engineering",
			bio: "Technology enthusiast focused on building scalable systems that make a difference.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<StakeholderGrid
	generating
	stakeholderType="investor"
	title="Backed by the best."
	subtitle="Point Nine, TSIC and others"
	stakeholders={[
		{
			name: "Point Nine Capital",
			image: "https://cdn.brandfetch.io/pointnine.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7"
		},
		{
			name: "TSIC Ventures",
			image: "https://cdn.brandfetch.io/tiny.vc/w/400/h/400/logo?c=1a2b3c4d5e"
		},
		{
			name: "Sequoia Capital",
			image: "https://cdn.brandfetch.io/sequoiacap.com/w/400/h/400/logo"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	generating
	title="Ready to collaborate?"
	subtitle="Let's create something amazing"
	description="Join the companies already leveraging our expertise to transform their digital presence and achieve their business goals."
/>
