<script lang="ts">
  const services = [
    {
      title: "Special Offers",
      description: "Adipisicing duis exercitation occaecat duis do ex aliquip tempor sit."
    },
    {
      title: "Frozen Food",
      description: "Officia incididunt cupidatat nulla irure non pariatur id consectetur officia."
    },
    {
      title: "Eggs and Cheese",
      description: "Consequat minim eiusmod nostrud non proident nisi ad ullamco occaecat nostrud."
    }
  ];
  console.log(services[0]);
</script>

<div class="flex justify-around w-4/5 gap-10">
  {#each services as service (service.title)}
    <div class="bg-gray-100 basis-1/3 px-4 py-8 space-y-10">
      <div class="h-20 w-20 bg-lime-700 rounded-full" />
      <p class="text-lime-800 text-4xl font-semibold">{service.title}</p>
      <p class="italic text-gray-900 leading-relaxed text-xl">{service.description}</p>
    </div>
  {/each}
</div>
