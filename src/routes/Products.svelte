<script>
  import farmer from "$lib/assets/farmer-lg.jpg";
  import cheese from "$lib/assets/cheese-lg.jpg";
  import vegetables from "$lib/assets/vegetables-lg.jpg";

  const products = [
    {
      title: "Vegetable boxes",
      description: "A selection of fresh, seasonal produce delivered straight to your door.",
      image: vegetables
    },
    {
      title: "Our Cheese",
      description: "We love our cheeses, and would be happy to put together a selection for you. Let us know how much",
      image: cheese
    },
    {
      title: "Our Farm",
      description: "A selection of fresh, seasonal produce delivered straight to your door.",
      image: farmer
    }
  ];
</script>

<div class="grid grid-cols-6 lg:grid-cols-3 w-11/12 lg:w-4/5  lg:gap-20">
  {#each products as product (product.title)}
    <div class="bg-indigo-800 w-full mb-36 lg:mb-0 lg:col-span-1 col-span-full h-96 relative">
      <img
        decoding="async"
        loading="lazy"
        src={product.image}
        alt=""
        class="absolute object-cover top-0 left-0 w-full h-full"
      />
      <div class="absolute -bottom-20  lg:left-7 w-[325px] p-7 bg-green-100 h-52">
        <p class="text-gray-900 text-4xl capitalize mb-5 ">{product.title}</p>
        <p class="text-lg">{product.description}</p>
      </div>
    </div>
  {/each}
</div>
