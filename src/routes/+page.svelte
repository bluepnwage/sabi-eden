<script lang="ts">
  import Services from "./Services.svelte";
  import Fruits from "./Fruits.svelte";
  import Products from "./Products.svelte";
  import "../app.css";

  //assets
  import mainBg from "$lib/assets/main-lg.jpg";
  import apples from "$lib/assets/apples-lg.jpg";
  import blueberries from "$lib/assets/blueberries-lg.jpg";
  import farmer from "$lib/assets/farmer-2-lg.jpg";
  import logo from "$lib/assets/logo.png";
</script>

<svelte:head>
  <title>Sabi's Eden</title>
</svelte:head>

<section class="h-screen px-10 flex flex-col lg:px-36 relative justify-center mb-36">
  <div class="absolute top-0 left-0 bg-black -z-10 w-full h-full">
    <img src={mainBg} alt="" class="opacity-50 object-cover  w-full h-full" />
  </div>

  <div class="lg:w-3/5">
    <img decoding="async" loading="lazy" src={logo} alt="" width="200" height="auto" />
    <h1 class="font-serif text-8xl text-white my-2">Organic</h1>
    <hr class="h-2 bg-white w-full mb-10" />
    <p class="text-white text-2xl mb-10">
      A selection of fresh, seasonal produce delivered straight <br /> to your door.
    </p>
    <button class="block px-8 py-4 text-gray-900  uppercase bg-white w-full lg:w-fit">More information</button>
  </div>
</section>

<section class="mb-36 flex flex-col items-center text-gray-900">
  <header class="w-11/12 lg:w-3/5 mb-10">
    <h2 class="font-serif text-7xl capitalize text-center mb-10">About us</h2>

    <p class="text-center italic text-gray-900">
      Buy seasonal organic recipe boxes, fruit & veg online at Riverford & order fresh organic meat from our expert
      butchers. Organic farming is an alternative food production method which prioritises sustainable production
      practices, respectful use of the countryside and concern for animal welfare.
    </p>
  </header>
  <Services />
</section>

<section class="flex flex-col items-center mb-36">
  <header class="bg-gray-100 w-11/12 lg:w-4/6 px-10 lg:px-20 py-10 text-center">
    <h2 class="font-serif text-7xl">Seasonal Fruits</h2>
    <hr class="h-1 bg-lime-600 w-1/12 mx-auto mb-7" />
    <p class="italic text-lg">
      Organic food is food produced by methods that comply with the standards of organic farming.
    </p>
  </header>
  <Products />
</section>

<section class="px-5 lg:px-36 py-10 relative">
  <div class="absolute bg-black -z-10 top-0 left-0 w-full h-full">
    <img class="w-full h-full object-cover opacity-30" src={apples} alt="" />
  </div>
  <h2 class="text-white font-serif text-6xl lg:text-8xl mb-10">Wholesale</h2>
  <p class="lg:w-3/5 text-gray-100 text-2xl lg:text-4xl leading-relaxed mb-10">
    To qualify for wholesale pricing you must buy from us in bulk quantities. For some customers that might be a pallet
    of lemons, or for others it could be a 10kg box of carrots for juicing at home.
  </p>
  <button class="bg-lime-600 text-gray-100 px-8 py-2  font-bold uppercase">Buy Online</button>
</section>
<section class="flex flex-col items-center mb-20">
  <header class="bg-gray-200 w-11/12 lg:w-4/6 py-20 px-5 lg:px-16 text-center">
    <h2 class="font-serif text-6xl capitalize mb-2">Seasonal fruits & veg</h2>
    <hr class="w-10 h-1 bg-lime-700 mx-auto mb-10" />
    <p class="italic text-lg">
      Organic food is food produced by methods that comply with the standards of organic farming.
    </p>
  </header>
  <Fruits />
</section>

<section class="px-10 lg:px-36 py-10 relative mb-48">
  <div class="absolute top-0  -z-10 left-0 w-full h-full bg-black">
    <img src={blueberries} alt="" class="w-full opacity-50 h-full object-cover" />
  </div>
  <header class="lg:w-3/5 mb-10">
    <h2 class="capitalize font-serif text-7xl text-white mb-10">Contact us</h2>
    <p class="text-4xl text-gray-100 leading-relaxed">
      Get the latest stories about organic, nutrition, health and wellness in your inbox every week!
    </p>
  </header>
  <div class="flex flex-col gap-4 lg:flex-row">
    <input placeholder="Enter your Name" class="appearance-none outline-none px-6 py-3" />
    <input placeholder="Enter your Email" class="appearance-none outline-none px-6 py-3" />
    <button class="py-3 px-6 uppercase bg-lime-600 text-gray-100 font-semibold">Submit</button>
  </div>
</section>

<section class="flex flex-col items-center mb-36">
  <header class="border-l-8 border-lime-700 w-11/12 lg:w-4/5 px-5 lg:px-20 py-4 relative">
    <h2 class="font-serif text-7xl mb-5 relative">How do you Know it's Organic</h2>
    <p class="text-xl relative">
      All pre-packaged organic food products in Europe which meet organic standards carry the “Euro-Leaf” EU organic
      logo. The logo also helps you to identify the place of farming e.g. Quisque fringilla sit amet dolor commodo
      efficitur. Aliquam et sem odio. In ullamcorper nisi nunc, et molestie ipsum iaculis sit amet.
    </p>
    <div class="absolute -top-16  right-0 -z-10 bg-gray-200 hidden lg:block h-96 w-[42%]" />
  </header>
</section>

<section class="w-full farmer-image">
  <img src={farmer} alt="" loading="lazy" decoding="async" class="w-full h-full object-contain  lg:object-cover" />
</section>

<footer class="py-16 flex flex-col border-t items-center">
  <div class="w-11/12 lg:w-4/5 gap-5 lg:gap-0 flex flex-col items-center lg:flex-row justify-between">
    <p class="text-gray-500 text-lg">© 2022, Sabi's Eden. All rights reserved</p>
    <div class="flex gap-4">
      <a aria-label="View facebook page" href="https://www.facebook.com/sabi.eden" rel="noreferrer" target="_blank">
        <svg xmlns="http://www.w3.org/2000/svg" class="stroke-gray-500" width="30" height="30" viewBox="0 0 24 24"
          ><g stroke-linejoin="round" stroke-linecap="round" stroke-width="2" fill="none"
            ><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path
              d="M7 10v4h3v7h4v-7h3l1-4h-4V8a1 1 0 0 1 1-1h3V3h-3a5 5 0 0 0-5 5v2H7"
            /></g
          ></svg
        >
      </a>
      <a aria-label="View instagram page" href="https://www.instagram.com/sabi_eden/" rel="noreferrer" target="_blank">
        <svg xmlns="http://www.w3.org/2000/svg" class="stroke-gray-500" width="30" height="30" viewBox="0 0 24 24"
          ><g stroke-linejoin="round" stroke-linecap="round" stroke-width="2" fill="none"
            ><path stroke="none" d="M0 0h24v24H0z" fill="none" /><rect
              x="4"
              y="4"
              width="16"
              height="16"
              rx="4"
            /><circle cx="12" cy="12" r="3" /><path d="M16.5 7.5v.001" /></g
          ></svg
        >
      </a>
    </div>
  </div>
</footer>

<style>
  button {
    letter-spacing: 2px;
  }
  .farmer-image {
    height: 80vh;
  }
  @media only screen and (max-width: 769px) {
    .farmer-image {
      height: fit-content;
    }
  }
</style>
