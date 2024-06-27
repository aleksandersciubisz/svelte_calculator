 <script>
    import { count } from '../stores/store';
    let inputValue = '';
  
    function handleKeyPress(event) {
      if (event.key === 'Enter') {
        const newValue = parseFloat(inputValue);
        if (!isNaN(newValue)) {
          count.set(newValue);
        }
        inputValue = '';
      }
    }
  </script>

<div class="border">
 
  
  <input 
    type="number" 
    bind:value={inputValue} 
    on:keypress={handleKeyPress} 
    placeholder="enter num"
  />
</div>

<style>
  .border {
    width: 40vw;
    height: 20vh;
    border: 3px solid var(--lr);
    margin: 5vw;

    display: flex;
    align-items: center;
    justify-content: center;
  }

  input {
    width: 90%;
    height: var(--g4);
    background-color: transparent;
    font-size: var(--g2);
    border: none;
    outline: none;
  }
</style>