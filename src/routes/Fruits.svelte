<script lang="ts">
  const fruits = Array(6).fill(null);
</script>

<div class="grid grid-cols-3 w-4/5 gap-5">
  {#each fruits as fruit, index (index)}
    <div class="bg-blue-800 h-72" />
  {/each}
</div>
