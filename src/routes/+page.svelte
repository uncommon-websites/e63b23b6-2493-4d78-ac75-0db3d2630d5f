<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";

	// Icons
	import IconMessageCircle from "~icons/lucide/message-circle";
	import IconZap from "~icons/lucide/zap";
	import IconMousePointer from "~icons/lucide/mouse-pointer";
	import IconUsers from "~icons/lucide/users";
	import IconPuzzle from "~icons/lucide/puzzle";
	import IconCalendar from "~icons/lucide/calendar";
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
	title="Validate product ideas with real users. In hours, not weeks."
	text="Series A product teams move fast—but most user research doesn't. Our platform replaces slow, expensive methods with on-demand feedback from real users, so you can validate new features with confidence in under 24 hours."
/>

<Testimonials
	testimonials={[
		{
			name: "Priya Chen",
			position: "Senior Product Manager",
			company: "StreamFlow Analytics",
			quote:
				"We cut feature validation time from 6 weeks to 3 days. The real user data helped us avoid a costly pivot that would have wasted 4 months of development.",
			image: "/generated/image-professional-asian-woman-product-manager.webp"
		},
		{
			name: "Marcus Williams",
			position: "VP of Product",
			company: "TechScale Solutions",
			quote:
				"Reduced our user research costs by 75% while getting 10x more reliable data. Our last three feature launches hit adoption targets within the first month.",
			image: "/generated/image-professional-black-man-product-manager-w.webp"
		},
		{
			name: "Sofia Rodriguez",
			position: "Head of Product Strategy",
			company: "GrowthEngine",
			quote:
				"Eliminated the guesswork that led to our biggest product failure. Now we validate with confidence before investing engineering resources — saved us $2M this year.",
			image: "/generated/image-professional-hispanic-woman-product-mana.webp"
		}
	]}
/>

<Features
	title="Validate features with confidence"
	subtitle="Turn user insights into product decisions that drive growth"
	features={[
		{
			title: "Real-time user feedback",
			description: "Capture authentic user reactions as they interact with your features. Get instant insights that traditional surveys miss.",
			icon: IconMessageCircle
		},
		{
			title: "Rapid prototype testing",
			description: "Test concepts in minutes, not weeks. Validate ideas before development starts and save engineering resources.",
			icon: IconZap
		},
		{
			title: "Behavioral analytics",
			description: "See exactly how users navigate your features. Identify friction points and optimize user flows with precision.",
			icon: IconMousePointer
		},
		{
			title: "Segmented insights",
			description: "Filter feedback by user type, usage patterns, and demographics. Make targeted improvements that matter most.",
			icon: IconUsers
		},
		{
			title: "Integration ready",
			description: "Connect with your existing product stack. Sync insights directly to Jira, Linear, or your preferred project management tool.",
			icon: IconPuzzle
		},
		{
			title: "Automated reporting",
			description: "Weekly summaries delivered to your inbox. Share compelling data stories with stakeholders and secure buy-in faster.",
			icon: IconCalendar
		}
	]}
/>
<AboutTeaser generating />
<CallToAction generating />
