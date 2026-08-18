<script lang="ts">
  interface Props {
    href?: string;
  }

  let { href = '/' }: Props = $props();
</script>

<a {href} aria-label="Example, home"><span aria-hidden="true">E</span>Example</a>

<style>
  a {
    display: inline-flex;
    align-items: center;
    gap: 0.625rem;
    color: inherit;
    font-weight: 700;
    text-decoration: none;
  }

  span {
    display: grid;
    width: 2rem;
    height: 2rem;
    place-items: center;
    border-radius: 50%;
    color: var(--example-color-paper);
    background: var(--example-color-ink);
    box-shadow: 3px 3px 0 var(--example-color-accent);
  }
</style>
