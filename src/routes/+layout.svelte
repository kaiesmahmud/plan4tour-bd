<script>
    import "../app.postcss";
    import "../app.css";
    import Footer from "../lib/components/ui/Footer.svelte";
    import Navbar from "../lib/components/ui/Navbar.svelte";
</script>
<div class=" relative w-full text-white overflow-hidden min-h-screen">
  <Navbar/>
    <slot />
  <Footer/>
  <div class="absolute shade-1 bg-teal-400/50 left-1 opacity-40 " />
  <div class='absolute gradient-01 opacity-50 left-1 ' />
  <div class='absolute gradient-02 opacity-50 bottom-4 left-1' />
  <div class='absolute gradient-03 opacity-50 right-1 top-[50%] ' />
  <div class='absolute gradient-04 opacity-30 top-10 right-[50%] ' />
</div>
