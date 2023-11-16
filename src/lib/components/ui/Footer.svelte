<script>
    import Icon from '@iconify/svelte';
    let paymentsimg = [
        {
            url : "https://www.gozayaan.com/img/icon-footer-bkash.a929cde0.svg",
            alt: "Bkash Img"
        },
        {
            url : "https://www.gozayaan.com/img/icon-payment-nagad.2e467251.svg",
            alt: "Nagad Img"
        },
        {
            url : "https://www.gozayaan.com/img/icon-payment-upay.fbd2acc5.svg",
            alt: "Upay Img"
        },
        {
            url : "https://www.gozayaan.com/img/icon-footer-visa.0cc68109.svg",
            alt: "Visa Card Img"
        },
        {
            url : "https://www.gozayaan.com/img/icon-footer-amex.a8ead788.svg",
            alt: "Amex Card Img"
        },
        {
            url : "https://www.gozayaan.com/img/icon-footer-mastercard.afdd5b7f.svg",
            alt: "Master Card Img"
        },
        {
            url : "https://www.gozayaan.com/img/icon-payment-dbbl.0975a769.svg",
            alt: "DBBL Card Img"
        },
        
        {
            url : "https://www.gozayaan.com/img/icon-payment-union.d875933a.svg",
            alt: "Union Img"
        },
        {
            url : "https://www.gozayaan.com/img/icon-payment-tap.dcf016e9.svg",
            alt: "Tap Img"
        },
    ]
    let discoverLinksStyle="hover:underline hover:texts-white/90 transition-all ease-in"
</script>

<div class="flex flex-col items-center justify-center p-5 bg-white/10">
    <div class="w-full flex flex-col lg:flex-row  gap-3 ">
        <div class=" capitalize flex flex-col md:flex-row  w-full lg:w-1/2">
            <div class=" block w-full md:w-1/2 pl-5 my-5">
                <h3>Discover</h3>
                <div class="flex flex-col gap-4 p-3 md:-5">
                    <a href="/" class={discoverLinksStyle}>Home</a>
                    <a href="/" class={discoverLinksStyle}>Hotels</a>
                    <a href="/" class={discoverLinksStyle}>Places</a>
                    <a href="/" class={discoverLinksStyle}>blogs</a>
                    <a href="/" class={discoverLinksStyle}>Products</a>
                </div>
            </div>
            <div class=" block w-full md:w-1/2  md:border-l pl-5 my-5">
                <h3>Payment Methods</h3>
                <div class=" inline-block">
                    <div class="grid grid-cols-3 gap-y-1  gap-x-3">
                        {#each paymentsimg as img }
                            <img class="w-20 h-20 rounded shadow" src={img.url} alt={img.alt}>
                        {/each}
                    </div>
                </div>
            </div>
        </div>
        <div class=" capitalize flex flex-col md:flex-row w-full lg:w-1/2">
            <div  class=" block w-full md:w-2/3 pl-5 my-5">
                <h3>Contact</h3>
                <div class="flex flex-col gap-3 my-5">
                    <a href="mailto:plan4tour.com@gmail.com">plan4tour.com@gmail.com</a>
                    <a href="tel:+8801846576185">+8801846576185</a>
                </div>
                <div class="flex gap-5 text-4xl">
                    <a href="/" class="hover:text-blue-500 p-3 bg-slate-600 hover:bg-white rounded-full transition-all ease-in">
                        <Icon icon="ic:outline-facebook"  />
                    </a>
                    <a href="/" class="hover:text-red-500 p-3 bg-slate-600 hover:bg-white rounded-full transition-all ease-in">
                        <Icon icon="mingcute:youtube-fill" />
                    </a>
                    <a href="/" class="hover:text-pink-500 p-3 bg-slate-600 hover:bg-white rounded-full transition-all ease-in">
                        <Icon icon="mdi:instagram" />
                    </a>
                </div>
            </div>
            <div  class=" block w-full md:w-1/3 pl-5 md:border-l my-5">
                <h3>Need Help?</h3>
                <p class="p-5">We are Always here for you! Knock us on Messenger anytime or Call our Hotline (10AM - 10PM).</p>
            </div>
        </div>
    </div>
    <footer class="flex flex-wrap justify-between items-center w-full text-cyan-500">
        <p class="font-light  text-xl">Plan4Tour.com</p>
        <p class="text-sm">
            Copyright 2023 All Right Reserved !
        </p>
    </footer>
</div>