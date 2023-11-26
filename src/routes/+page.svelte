<script>
    import 'swiper/css';
    import'swiper/css/navigation';
    import'swiper/css/pagination';
    import'swiper/css/scrollbar';
    import'swiper/css/effect-fade';

	import FAQ from '../lib/components/FAQ.svelte';
    import HeroSection from '../lib/components/HeroSection.svelte';
    // import TestCarousel from '../lib/components/TestCarousel.svelte';
    // import Carousel from 'svelte-carousel'
</script>
<svelte:head>
    <title>Plan4Tour </title> 
	<meta name="description" content="Experience effortless page name editing with the Drag-N-Drop Page Name Editor in SvelteKit by Kaies Mahmud Nehal. Seamlessly designed using Tailwind CSS and Svelte-DND-Action, enriched with Iconify icons. Elevate your web development with intuitive drag-and-drop functionality. Unlock user-friendly design and efficiency in one powerful tool" />
</svelte:head>
<!-- <TestCarousel/> -->
<HeroSection/>
<h1 class="text-4xl text-center p-2">Welcome to SvelteKit</h1>
<FAQ />
