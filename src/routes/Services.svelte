<script lang="ts">
  import broccoli from "$lib/assets/broccoli.png";
  import fish from "$lib/assets/fish.png";
  import cheese from "$lib/assets/cheese.png";
  const services = [
    {
      title: "Special Offers",
      description: "Adipisicing duis exercitation occaecat duis do ex aliquip tempor sit.",
      icon: broccoli
    },
    {
      title: "Frozen Food",
      description: "Officia incididunt cupidatat nulla irure non pariatur id consectetur officia.",
      icon: fish
    },
    {
      title: "Eggs and Cheese",
      description: "Consequat minim eiusmod nostrud non proident nisi ad ullamco occaecat nostrud.",
      icon: cheese
    }
  ];
</script>

<div class="flex flex-col lg:flex-row justify-around w-11/12 lg:w-4/5 gap-10">
  {#each services as service (service.title)}
    <div class="bg-gray-100 basis-1/3 px-4 py-8 space-y-10">
      <div class="h-20 w-20 bg-lime-700 flex justify-center items-center rounded-full">
        <img decoding="async" loading="lazy" src={service.icon} width="50" height="50" alt="" />
      </div>
      <p class="text-lime-800 text-4xl font-semibold">{service.title}</p>
      <p class="italic text-gray-900 leading-relaxed text-xl">{service.description}</p>
    </div>
  {/each}
</div>
