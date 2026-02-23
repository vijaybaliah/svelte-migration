<script lang="ts">
  let count = 0;     // Svelte 5 runes syntax
  export let label = 'Click me';

  const handleClick = () => {
    count += 1;
  };
</script>

<button on:click={handleClick}>
  {label} ({count})
</button>
