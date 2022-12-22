<script>
  const products = [
    {
      title: "Vegetable boxes",
      description: "A selection of fresh, seasonal produce delivered straight to your door."
    },
    {
      title: "Our Cheese",
      description: "We love our cheeses, and would be happy to put together a selection for you. Let us know how much"
    },
    {
      title: "Our Farm",
      description: "A selection of fresh, seasonal produce delivered straight to your door."
    }
  ];
</script>

<div class="grid grid-cols-3 w-5/6 gap-20">
  {#each products as product (product.title)}
    <div class="bg-indigo-800 h-96 relative">
      <div class="absolute -bottom-20  left-7 w-[325px] p-7 bg-green-100 h-52">
        <p class="text-gray-900 text-4xl capitalize mb-5 ">{product.title}</p>
        <p class="text-lg">{product.description}</p>
      </div>
    </div>
  {/each}
</div>
