<script>
  let count_value
  
  import { count } from '../stores/stores.js'
  import Incrementer from './Incrementer.svelte'
  import Decrementer from './Decrementer.svelte'
  import Resetter from './Resetter.svelte'

  const unsubscribe = count.subscribe(value => {
    count_value = value
  })
</script>

<h1> The count is {count_value} </h1>
<Incrementer/>
<Decrementer/>
<Resetter/>
