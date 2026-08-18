<script lang="ts">
  import { BrandMark, ThemeToggle } from '$lib';
</script>

<svelte:head><title>Example brand kit</title></svelte:head>

<main>
  <p class="eyebrow">Brand toolkit</p>
  <BrandMark />
  <h1>Example</h1>
  <p>Shared brand identity, design tokens, and reusable Svelte components.</p>
  <ThemeToggle />
</main>

<style>
  main {
    width: min(calc(100% - 3rem), 72rem);
    margin: 0 auto;
    padding: 6rem 0;
  }

  .eyebrow {
    color: var(--example-color-muted);
    font-family: var(--example-font-mono);
    font-size: 0.75rem;
    letter-spacing: 0.14em;
    text-transform: uppercase;
  }

  h1 {
    margin: 4rem 0 1rem;
    font-size: clamp(4rem, 12vw, 10rem);
    line-height: 0.85;
    letter-spacing: -0.06em;
  }
</style>
