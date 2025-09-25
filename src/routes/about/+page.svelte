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
			title: "Speed is strategy",
			description: "In early-stage SaaS, faster feedback means better decisions. We help product teams validate features in hours—not weeks."
		},
		{
			title: "Signal over noise",
			description: "We deliver insights that move the roadmap forward. No fluff, no guesswork—just the truth from real users."
		},
		{
			title: "Built for builders",
			description: "Our tools are made for product leaders who want to stay close to their users and ship what truly matters."
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
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Our team."
	subtitle="Your partners in product validation."
	stakeholders={[
		{
			name: "Jorge Dobón",
			position: "Managing Partner",
			bio: "Experienced leader driving product innovation with deep expertise in user research and validation methodologies.",
			image: "/generated/image-a-professional-businessman-in-his-30s-ph.webp"
		},
		{
			name: "Mario Navarro",
			position: "Partner & IC Member",
			bio: "Strategic partner focused on building scalable research solutions that deliver actionable insights to product teams.",
			image: "/generated/image-a-professional-businesswoman-in-her-40s-.webp"
		},
		{
			name: "Julio Ribes",
			position: "Partner & IC Member",
			bio: "Product research specialist with extensive experience in fast-moving startup environments and user validation frameworks.",
			image: "/generated/image-a-professional-businessman-in-his-50s-ca.webp"
		},
		{
			name: "Álvaro Callejo",
			position: "Partner & IC Member",
			bio: "Technology and product development expert committed to transforming how teams gather and act on user feedback.",
			image: "/generated/image-a-professional-businessman-in-his-late-2.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Start testing today"
	subtitle="Get answers in 24 hours"
	description="Join top product teams moving faster and smarter—no contracts, no waiting. See your first user insights tomorrow and make confident product decisions."
	imageSrc="/generated/image-a-professional-product-manager-dressed-i.webp"
/>
