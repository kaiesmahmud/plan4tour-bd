<script>
    import "../app.postcss";
    import "../app.css";
    import Footer from "../lib/components/Footer.svelte";
    import Navbar from "../lib/components/Navbar.svelte";
</script>
<div class=" relative w-full text-white overflow-hidden min-h-screen">
  <Navbar/>
  <div class="mt-6 md:mt-20">
    <slot />
  </div>
  <Footer/>
  <!-- <div class="absolute shade-1 bg-teal-400/50 left-1 opacity-40 " /> -->
  <!-- <div class='absolute gradient-01 opacity-50 left-1 ' /> -->
  <!-- <div class='absolute gradient-02 opacity-50 bottom-4 left-1' /> -->
  <!-- <div class='absolute gradient-03 opacity-50 right-1 top-[50%] ' /> -->
  <div class='absolute w-[200px] h-[200px] md:w-[400px] md:h-[400px] gradient-04 opacity-50 md:opacity-30 top-0 left-0 gradient-animation' />
</div>
