<script lang="ts">
  import { Counter } from "$lib";
  import Services from "./Services.svelte";
  import Fruits from "./Fruits.svelte";
  import "../app.css";
</script>

<section class="h-screen bg-indigo-900 flex flex-col px-36 justify-center mb-36">
  <div class="w-3/5">
    <div class="h-36 w-36 rounded-full border-2 mb-10 flex items-center justify-center border-gray-100" />
    <h1 class="font-serif  text-8xl text-white mb-2">Organic</h1>
    <hr class="h-2 bg-white w-full mb-10" />
    <p class="text-white text-2xl mb-10">
      A selection of fresh, seasonal produce delivered straight <br /> to your door.
    </p>
    <button class="block px-8 py-4 text-gray-900  uppercase bg-white w-fit">More information</button>
  </div>
</section>
<section class="mb-36 flex flex-col items-center text-gray-900">
  <header class="w-3/5 mb-10">
    <h2 class="font-serif text-7xl capitalize text-center mb-10">About us</h2>

    <p class="text-center italic text-gray-900">
      Buy seasonal organic recipe boxes, fruit & veg online at Riverford & order fresh organic meat from our expert
      butchers. Organic farming is an alternative food production method which prioritises sustainable production
      practices, respectful use of the countryside and concern for animal welfare.
    </p>
  </header>
  <Services />
</section>
<section class="bg-indigo-800 px-36 py-10 ">
  <h2 class="text-white font-serif text-8xl mb-10">Wholesale</h2>
  <p class="w-3/5 text-gray-100 text-4xl leading-relaxed mb-10">
    To qualify for wholesale pricing you must buy from us in bulk quantities. For some customers that might be a pallet
    of lemons, or for others it could be a 10kg box of carrots for juicing at home.
  </p>
  <button class="bg-lime-600 text-gray-100 px-8 py-2  font-bold uppercase">Buy Online</button>
</section>
<section class="flex flex-col items-center mb-20">
  <header class="bg-gray-200 w-4/6 py-20 px-16 text-center">
    <h2 class="font-serif text-6xl capitalize mb-2">Seasonal fruits & veg</h2>
    <hr class="w-10 h-1 bg-lime-700 mx-auto mb-10" />
    <p class="italic text-lg">
      Organic food is food produced by methods that comply with the standards of organic farming.
    </p>
  </header>
  <Fruits />
</section>
<section class="px-36 py-10 bg-indigo-800 mb-20">
  <header class="w-3/5 mb-10">
    <h2 class="capitalize font-serif text-7xl text-white mb-10">Contact us</h2>
    <p class="text-4xl text-gray-100 leading-relaxed">
      Get the latest stories about organic, nutrition, health and wellness in your inbox every week!
    </p>
  </header>
  <div class="space-x-4">
    <input placeholder="Enter your Name" class="appearance-none outline-none px-6 py-3" />
    <input placeholder="Enter your Email" class="appearance-none outline-none px-6 py-3" />
    <button class="py-3 px-6 uppercase bg-lime-600 text-gray-100 font-semibold">Submit</button>
  </div>
</section>

<style>
  button {
    letter-spacing: 2px;
  }
</style>
