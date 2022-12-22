<script>
  let counter = 0;
  const increment = () => (counter += 1);
</script>

<p>{counter}</p>
<button class="border px-4 py-2 rounded-md font-semibold bg-indigo-600 text-gray-100" on:click={increment}>
  Increment
</button>
