<script>
import {count} from "../stores/store.js"

function add() {
  count.update((n)=> n+1)
}

function minus() {
  count.update((n)=> n-1)
}

function mul() {
  count.update((n)=> n*2)
}

function div() {
  count.update((n)=> n/2)
}
</script>

<div class="border">
  <button  on:click={add}>+</button>
  <button  on:click={minus}>-</button>
  <button  on:click={mul}>*</button>
  <button  on:click={div}>/</button>
</div>

<style>
  .border {
    width: 40vw;
    height: 50vh;
    margin: 5vw;


    display:grid;
    grid-template-columns: 1fr 1fr;
    column-gap: var(--g0);
  }

  button {
    font-size: var(--g2);
    font-weight: 900;
  }
</style>