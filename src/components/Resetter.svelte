<script>
  import { count } from '../stores/stores.js'

  function decrement() {
    count.set(0)
  }
</script>

<button on:click={ decrement }>
  Reset
</button>