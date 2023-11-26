<script>
    import Carousel from 'svelte-carousel'
    let demos = [0,0,0,0]
    let imgSlides = [
        {
            url: "https://images.unsplash.com/photo-1465778893808-9b3d1b443be4?q=80&w=2075&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
        },
        {
            url: "https://images.unsplash.com/photo-1615277716590-d87d101caa70?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
        },
        {
            url: "https://images.unsplash.com/photo-1482332486572-10fff1bedfbe?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
        },
        
        
        
    ]
    // import {Swiper,SwiperSlide} from 'swiper';
</script>

<svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/swiper@8.2.4/swiper-bundle.css"/>
</svelte:head>

<div class="min-h-screen" >
    <div class=" w-full    overflow-hidden flex items-center justify-center">
        <img  src="/plan4tour-1.jpeg" class="w-full md:w-[80%] rounded" alt="">
    </div>
    <h1 class=" text-center">Hero SEction Here</h1>
    <p class=" text-center">Will Be Updating</p>
    <div class="p-5">
        <!-- <Swiper>
            <SwiperSlide>a</SwiperSlide>
            <SwiperSlide>b </SwiperSlide>
            <SwiperSlide>c</SwiperSlide>
            <SwiperSlide>d</SwiperSlide>
        </Swiper> -->
        <!-- <Carousel
        autoplay
        autoplayDuration={2000}
        dots={false}
        arrows={false}
        >
            <div class="w-full p-5">
                <img  src="https://images.unsplash.com/photo-1503220317375-aaad61436b1b?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" class="w-full" alt="">
            </div>
            <div class="w-full p-5">
                <img  src="https://images.unsplash.com/photo-1503220317375-aaad61436b1b?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" class="w-full" alt="">
            </div>
            <div class="w-full p-5">
                <img  src="https://images.unsplash.com/photo-1503220317375-aaad61436b1b?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" class="w-full" alt="">
            </div>
        </Carousel> -->

    </div>

</div>

