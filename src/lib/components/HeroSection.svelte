<script>
        import Icon from '@iconify/svelte';

    // import {Swiper,SwiperSlide} from 'swiper';
    const Services = [
        {
            id: '01',
            title: "Hotels",
            icon: "carbon:hotel",
            url: "/hotels",
            description: "Compare hotel prices and find the best deals"

        },
        {
            id: '02',
            title: "Tour Places",
            icon: "mdi:place-outline",
            url: "/touring-places",
            description: "Let us guide you through the wonders of the world"
        },
        {
            id: '03',
            title: "Tour Blogs",
            icon: "carbon:blog",
            url: "/tour-blogs",
            description: "Let our travel tales ignite your passion for adventure"
        },
        {
            id: '04',
            title: "Travel Tickets",
            icon: "ion:ticket-outline",
            url: "/travel-tickets",
            description: "Book your round-trip flights and save up to 50% with our special offers"
        },
    ]
</script>

<svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/swiper@8.2.4/swiper-bundle.css"/>
</svelte:head>

<div class="min-h-screen" >
    <div class=" w-full    overflow-hidden flex items-center justify-center">
        <img  src="/plan4tour-1.jpeg" class="w-full md:w-[80%] rounded" alt="">
    </div>
    <div>

    </div>
    <div class="w-full flex items-center justify-center mt-5 md:mt-10">
        <!-- <div class="p-5 w-full md:w-[70%] md:bg-black/90 flex items-center justify-center gap-3 rounded flex-col md:flex-row"> -->
        <div class="p-5 w-full md:w-[70%]  rounded grid grid-cols-2 md:grid-cols-4 gap-2 text-center">
            {#each Services as service(service.id)}
                <div class="bg-white/10 md:bg-white/20 rounded p-2 md:p-5 pt-4 flex flex-col items-center justify-between gap-3 md:gap-5">
                    <div>
                        <div class="text-center flex items-center flex-col gap-1">
                            <div class="text-3xl lg:text-5xl">
                                <Icon icon={service.icon} />
                            </div>
                            <p>{service.title}</p>
                        </div>
                        <p class="text-xs md:text-sm text-center text-white/50">{service.description}</p>
                    </div>
                    <a href={service.url} class="w-full bg-black/50 font-semibold rounded text-sm p-3 "> View Details</a>
                </div>
            {/each}
    
        </div>

    </div>
    <h1 class=" text-center">Hero SEction Here</h1>
    <p class=" text-center">Will Be Updating</p>

</div>

