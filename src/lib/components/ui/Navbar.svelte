<script>
    import Icon from '@iconify/svelte';
    import { writable } from 'svelte/store';
    let lang = 'en';
    const changeLang = (lan) => {
        if(lan != lang){
            console.log("changed to , ", lan)
            lang = lan ;
        }
    }
    let open = writable(false) ;
    const handleOpen = () => {
        console.log("Clicked")
        open.set(!$open) ;
    
    } ;
    
</script>
<div class="fixed top-0 left-0 backdrop-blur-2xl bg-white/10 w-full p-3 z-[100] flex justify-between lg:justify-around items-center flex-wrap md:flex-nowrap">
    <div class="text-3xl font-semibold order-1">
        <a href="/" >Plan4Tour</a>
    </div>
    <div class="order-3">
        <button class="text-5xl lg:hidden" on:click={handleOpen}>
            <Icon icon="jam:menu" />
        </button>
        
        <div class="hidden  lg:flex gap-3 ">
            <a href="/" class="p-3 bg-slate-200 text-black rounded flex items-center justify-center gap-3">
                <Icon icon="carbon:hotel" />
                Hotels
            </a>
            <a href="/" class="p-3 bg-pink-100 text-black rounded flex items-center justify-center gap-3">
                <Icon icon="mdi:place-outline" />
                Touring Places
            </a>
            <a href="/" class="p-3 bg-violet-100 text-black rounded flex items-center justify-center gap-3">
                <Icon icon="carbon:blog" />
                Tour Blogs
            </a>
            <a href="/" class="p-3 bg-green-500 text-black rounded flex items-center justify-center gap-3">
                <Icon icon="clarity:camera-line" />
                Need PhotoGrapher?
            </a>
        </div>
        
    </div>
    <div class=" order-2 lg:order-3 flex text-xs md:text-sm bg-white/50 p-1  rounded select-none cursor-pointer transition-all ease-in">
        <button on:click={()=>{changeLang('en')}} class={`${lang == 'en'?'bg-slate-700' : ' '} px-3 py-1 rounded`}>
            English
        </button>
        <button on:click={()=>{changeLang('bn')}}
            class={`${lang == 'bn'?'bg-slate-700' : ' '} px-3 py-1 rounded`}>Bangla
        </button>
    </div>
</div>

{#if $open}
    <div class="z-[200] fixed w-screen h-screen bg-black flex flex-col gap-10 ">
        <div class="flex w-full justify-end p-5">
            <button class="text-4xl" on:click={handleOpen}>
                <Icon icon="maki:cross" />
            </button>
        </div>
        <div class="flex flex-col items-center justify-center gap-3 w-full">
            <a href="/" class="p-3 bg-slate-200 text-black rounded flex items-center justify-center gap-3 w-2/3">
                <Icon icon="carbon:hotel" />
                Hotels
            </a>
            <a href="/" class="p-3 bg-pink-100 text-black rounded flex items-center justify-center gap-3 w-2/3">
                <Icon icon="mdi:place-outline" />
                Touring Places
            </a>
            <a href="/" class="p-3 bg-violet-100 text-black rounded flex items-center justify-center gap-3 w-2/3">
                <Icon icon="carbon:blog" />
                Tour Blogs
            </a>
            <a href="/" class="p-3 bg-green-500 text-black rounded flex items-center justify-center gap-3 w-2/3">
                <Icon icon="clarity:camera-line" />
                Need PhotoGrapher?
            </a>
        </div>
    </div>
{/if}
        
        
        