<script>
import Input from "./lib/Input.svelte";
import Keyboard from "./lib/Keyboard.svelte";
import Screen from "./lib/Screen.svelte";

</script>

<main>
<div class="col">
  <Input/>
  <Keyboard/>
</div>
<div class="col">
  <Screen/>
</div>
</main>

<style>
main {
  display: flex;
}


</style>
