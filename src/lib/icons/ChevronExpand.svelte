<script lang="ts">
  import type { SVGAttributes } from 'svelte/elements'

  let { ...props }: SVGAttributes<EventTarget> = $props()
</script>

<svg {...props} fill="currentColor" viewBox="0 0 16 16">
  <path
    d="M3.646 9.146a.5.5 0 0 1 .708 0L8 12.793l3.646-3.647a.5.5 0 0 1 .708.708l-4 4a.5.5 0 0 1-.708 0l-4-4a.5.5 0 0 1 0-.708zm0-2.292a.5.5 0 0 0 .708 0L8 3.207l3.646 3.647a.5.5 0 0 0 .708-.708l-4-4a.5.5 0 0 0-.708 0l-4 4a.5.5 0 0 0 0 .708z"
  />
</svg>
