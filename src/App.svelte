<script lang="ts">
import { Button, Icon, ButtonGroup, ButtonGroupItem } from "svelte-materialify";
import { mdiHeart } from "@mdi/js";
export let name: string;
let value = 1;
</script>

<main>
  <h1>Hello {name}!</h1>
  <p>
    Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
    how to build Svelte apps.
  </p>
  <div class="text-center">
    <Button class="pink-text">
      <Icon path={mdiHeart} />
      Hello
    </Button>
    <ButtonGroup activeClass="primary-color" bind:value>
      <ButtonGroupItem>Left</ButtonGroupItem>
      <ButtonGroupItem>Center</ButtonGroupItem>
      <ButtonGroupItem>Right</ButtonGroupItem>
      <ButtonGroupItem>Justify</ButtonGroupItem>
    </ButtonGroup>
    <br />
    Value:
    {value}
  </div>
</main>

<style>
main {
  text-align: center;
  padding: 1em;
  max-width: 240px;
  margin: 0 auto;
}

h1 {
  color: #ff3e00;
  text-transform: uppercase;
  font-size: 4em;
  font-weight: 100;
}

@media (min-width: 640px) {
  main {
    max-width: none;
  }
}
</style>
