<script>
  import { Button } from 'forui'

  let name = 'unknown'
</script>

<p>this is {name}</p>
<Button on:click={() => (name = 'new')}>new</Button>
<Button on:click={() => (name = 'other')}>other</Button>
<Button on:click={() => (name = 'unknown')}>reset</Button>

<style>
  :global(button) {
    background: red;
  }
</style>
