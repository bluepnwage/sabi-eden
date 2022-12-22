<script lang="ts">
  import pumpkins from "$lib/assets/pumpkins-lg.jpg";
  import lettuce from "$lib/assets/lettuce-lg.jpg";
  import greenApples from "$lib/assets/green-apples.jpg";
  import carrots from "$lib/assets/carrots-lg.jpg";
  import apples from "$lib/assets/apples-lg.jpg";
  import blueberries from "$lib/assets/blueberries-lg.jpg";

  const fruits = [lettuce, greenApples, pumpkins, carrots, blueberries, apples];
</script>

<div class="grid grid-cols-6 lg:grid-cols-3 w-11/12 lg:w-4/5 gap-5">
  {#each fruits as fruit, index (index)}
    <img decoding="async" loading="lazy" src={fruit} class="h-96 object-cover col-span-full lg:col-span-1" alt="" />
  {/each}
</div>
