<script>
        import Icon from '@iconify/svelte';

    // import {Swiper,SwiperSlide} from 'swiper';
    const Services = [
        {
            id: '01',
            title: "Hotels",
            icon: "carbon:hotel",
            color:"text-cyan-300",
            url: "/hotels",
            description: "Compare hotel prices and find the best deals"

        },
        {
            id: '02',
            title: "Tour Places",
            icon: "mdi:place-outline",
            color:"text-pink-500",
            url: "/touring-places",
            description: "Let us guide you through the wonders of the world"
        },
        {
            id: '03',
            title: "Tour Blogs",
            icon: "carbon:blog",
            color:"text-blue-500",
            url: "/tour-blogs",
            description: "Let our travel tales ignite your passion for adventure"
        },
        {
            id: '04',
            title: "Travel Tickets",
            icon: "ion:ticket-outline",
            color:"text-green-500",
            url: "/travel-tickets",
            description: "Book your round-trip flights and save up to 50% with our special offers"
        },
    ]
    let textGradient = "text-transparent capitalize bg-clip-text bg-gradient-to-r from-purple-400 to-pink-600"
</script>

<svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/swiper@8.2.4/swiper-bundle.css"/>
</svelte:head>

<div class="min-h-screen" >
    <div class=" w-full    overflow-hidden flex items-center justify-center">
        <img  src="/plan4tour-1.jpeg" class="w-full md:w-[80%] rounded" alt="">
    </div>
    <div class="w-full flex items-center justify-center text-center">
        <div class="p-5 w-full md:w-[70%] ">
            <h2 class="py-5 text-transparent capitalize bg-clip-text bg-gradient-to-r from-purple-400 to-pink-600">
                Your one-stop destination for crafting unforgettable travel experiences. 
            </h2>
            <p class="text-xs md:text-sm text-white/80 p-5">
                At Plan4tour, we believe that travel is not just about ticking off destinations; it's about immersing yourself in new cultures, exploring hidden gems, and creating memories that will last a lifetime. That's why we've combined the expertise of seasoned travel agents with the passion of experienced tour guides to offer a comprehensive travel service that caters to every traveler's needs.
            </p>
        </div>
    </div>
    <div class="w-full flex items-center justify-center mt-5 md:mt-10">
        <!-- <div class="p-5 w-full md:w-[70%] md:bg-black/90 flex items-center justify-center gap-3 rounded flex-col md:flex-row"> -->
        <div class="p-5 w-full md:w-[70%]  rounded grid grid-cols-2 md:grid-cols-4 gap-2 text-center">
            {#each Services as service(service.id)}
                <div class="bg-white/10 md:bg-white/20 rounded p-2 md:p-5 pt-4 flex flex-col items-center justify-between gap-3 md:gap-5">
                    <div>
                        <div class="text-center flex items-center flex-col gap-1">
                            <div class={`text-3xl lg:text-5xl p-5 bg-black/50 rounded-full ${service.color}`}>
                                <Icon icon={service.icon} />
                            </div>
                            <p class="md:text-lg">{service.title}</p>
                        </div>
                        <p class="text-xs md:text-sm text-center text-white/50">{service.description}</p>
                    </div>
                    <a href={service.url} class="w-full bg-black/50 font-semibold rounded text-sm p-3 "> View Details</a>
                </div>
            {/each}
    
        </div>

    </div>
    <p class=" text-center">Will Be Updating</p>

</div>

