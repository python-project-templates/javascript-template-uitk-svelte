# @python-project-templates/uitk-svelte

Shared brand identity, design tokens, and reusable Svelte components.

See [`BRAND.md`](./BRAND.md) for the canonical brand guide.

## Install

```bash
pnpm add @python-project-templates/uitk-svelte
```

Import design tokens once at the application root:

```css
@import '@python-project-templates/uitk-svelte/tokens.css';
```

```svelte
<script lang="ts">
  import { BrandMark, ThemeToggle } from '@python-project-templates/uitk-svelte';
</script>

<BrandMark />
<ThemeToggle />
```

## Develop

```bash
pnpm install
pnpm dev
pnpm check
pnpm lint
pnpm fix
pnpm test
pnpm build
```

After customizing the showcase, run `pnpm test:e2e:update` once to establish its visual baseline.
