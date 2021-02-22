<script lang="ts">
import { Button } from "svelte-materialify";
</script>

<Button size="x-large" class="green white-text">Hello</Button>

<style global lang="postcss">
/* only apply purgecss on utilities, per Tailwind docs */
/* purgecss start ignore */
@tailwind base;
@tailwind components;
/* purgecss end ignore */

@tailwind utilities;
</style>
