<script>
    import { Navigation, Pagination, A11y } from 'swiper';
    import { Swiper, SwiperSlide } from 'swiper';
  
      let swiper;
  </script>
  
  <svelte:head>
      <link rel="stylesheet" href="https://unpkg.com/swiper@8.2.4/swiper-bundle.css"/>
  </svelte:head>
  
  <Swiper modules={[Navigation, Pagination, A11y]}
                  slidesPerView={1} navigation
                  on:swiper={e => swiper = e.detail[0]}>
      <SwiperSlide>Slide 1</SwiperSlide>
      <SwiperSlide>Slide 2</SwiperSlide>
      <SwiperSlide>Slide 3</SwiperSlide>
      <SwiperSlide>Slide 4</SwiperSlide>
  </Swiper>
  
  <button class="p-5 bg-green-500" type=button on:click={() => swiper.slidePrev()}>Previous</button>
  <button class="p-5 bg-green-500" type=button on:click={() => swiper.slideNext()}>Next</button>