<script lang="ts">
  import { page } from '$app/state'
  import { name } from '$root/package.json'
  import { DemoNav } from '$site'
  import { demos } from '$site/stores'
  import { PrevNext } from 'svelte-zoo'

  interface Props {
    children?: import('svelte').Snippet
  }
  let { children }: Props = $props()
</script>

<h1>
  <img src="favicon.svg" alt={name} height="50" width="50" />&ensp;Svelte MultiSelect
</h1>

<main>
  <DemoNav style="place-content: center;" />

  {@render children?.()}

  <PrevNext
    items={$demos}
    current={page.url.pathname}
    style="max-width: 55em; margin: auto;"
  />
</main>

<style>
  h1 {
    text-align: center;
    display: flex;
    place-content: center;
    place-items: center;
  }
</style>
