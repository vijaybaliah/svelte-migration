<script lang="ts">
  let count = 0;     // Svelte 5 runes syntax
  export let label = 'Click me';

  const handleClick = () => {
    count += 1;
  };
</script>

<button on:click={handleClick} class="button">
  {label} ({count})
</button>

<style lang="scss">
.button {
    appearance: none;
    background: #8937ee;
    outline: none;
    border: none;
    padding: 8px 16px;
    border-radius: 8px;
    color: white;
}
</style>