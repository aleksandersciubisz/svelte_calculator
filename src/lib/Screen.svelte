<script>
import {count} from "../stores/store.js"

let count_value;

count.subscribe((value) => {
  count_value = value;
});
</script>

<div class="border">
<h1>{count_value}</h1>
</div>

<style>
  .border {
    width: 40vw;
    height: 80vh;
    border: 3px solid var(--lr);
    margin: 5vw;

    display: flex;
    align-items: center;
    justify-content: center;
  }
</style>