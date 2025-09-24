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
	import IconBrain from "~icons/lucide/brain";
	import IconApple from "~icons/lucide/apple";
	import IconTrendingUp from "~icons/lucide/trending-up";
	import IconCalendar from "~icons/lucide/calendar";
	import IconUsers from "~icons/lucide/users";
	import IconEye from "~icons/lucide/eye";
</script>

<Hero
	title="One app for your entire fitness life"
	subtitle="Plan workouts. Track performance. Manage nutrition."
	imageSrc="/generated/image-professional-fitness-enthusiast-training.webp"
	centered={false}
/>
<LogoScroller label="" generating />

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	generating
	testimonials={[
		{
			name: "Jane Smith",
			position: "CTO",
			company: "Tech Innovations",
			quote:
				"Their cutting-edge automation boosted our productivity by 35%.\nThe intuitive interface reduced training time and improved team adoption.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "John Doe",
			position: "Director of Operations",
			company: "Global Solutions",
			quote:
				"Their robust security protocols gave us confidence in handling sensitive data.\nThe 24/7 support team resolved issues within hours, not days.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Sarah Johnson",
			position: "Product Manager",
			company: "Future Systems",
			quote:
				"The scalable platform grew seamlessly with our business needs.\nTheir customization options allowed us to tailor solutions perfectly to our workflows.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<Features
	title="Everything you need in one powerful platform"
	subtitle="From workout planning to nutritional analysis, FitHub transforms fragmented routines into cohesive progress that delivers real results."
	features={[
		{
			title: "AI-optimized workout planning",
			description: "Generate personalized 15-minute workouts that sync with your calendar. No more time commitment fears, just efficient results that fit your busy schedule.",
			icon: IconBrain
		},
		{
			title: "Real-time nutrition integration",
			description: "See exactly how your meals impact workout performance with synchronized nutritional analysis. Unlike fragmented apps, everything connects seamlessly.",
			icon: IconApple
		},
		{
			title: "Comprehensive performance analytics",
			description: "Track every metric that matters across strength, cardio, and recovery. Transform scattered data points into clear progress insights.",
			icon: IconTrendingUp
		},
		{
			title: "Smart calendar integration",
			description: "Automatically schedule workouts around meetings and commitments. Your fitness routine adapts to your life, not the other way around.",
			icon: IconCalendar
		},
		{
			title: "Personal trainer collaboration",
			description: "Share progress data and receive expert guidance remotely. Bridge the gap between independent training and professional coaching.",
			icon: IconUsers
		},
		{
			title: "Predictive health insights",
			description: "Anticipate performance trends and prevent overtraining with advanced analytics. Make smarter decisions about your fitness journey.",
			icon: IconEye
		}
	]}
/>
<AboutTeaser generating />
<CallToAction
	title="Start seeing progress that makes sense"
	subtitle="Join thousands of fitness enthusiasts"
	description="Stop juggling multiple apps that don't work together. FitHub connects your training, nutrition, and performance data in one intelligent platform—so you can make smarter decisions and see faster results."
	imageSrc="/generated/image-photorealistic-lifestyle-photo-of-a-happ.webp"
	callsToAction={[
		{
			href: "/get-started",
			label: "Start your free trial",
			variant: "primary"
		},
		{
			href: "/demo",
			label: "See how it works",
			variant: "secondary"
		}
	]}
/>
