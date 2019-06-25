<script>
  let name = 'unknown'
</script>

<p>this is {name}</p>
<button
  on:click={() => {
    name = 'new'
  }}>
  new
</button>
<button on:click={() => (name = 'other')}>other</button>
<button on:click={() => (name = 'unknown')}>reset</button>
