<Header>
  <h1 slot="left">{title}</h1>
  <div slot="center">
    <Input
      on:input={e => router.go({ query: e.detail })}
      value={$router.query}
      label="Search"
      valid={$router.query === 'cheat'}
      error={$router.query === 'error'}
      clean />
  </div>
  <nav slot="right">
    <BtnGroup>
      <Button icon flat clean on:click={() => ($tmp = 'a')}>
        <ActionToday />
      </Button>
      <Button icon flat clean on:click={() => ($tmp = 'b')}>
        <ActionDone />
      </Button>
      <Button icon flat clean on:click={() => ($tmp = 'c')}>
        <ActionSearch />
      </Button>
    </BtnGroup>
  </nav>
</Header>

<Main>
  <pre>$router: {JSON.stringify($router, null, 2)}</pre>
  <br />
  <Order />
</Main>

<script>
  import { tmp, title } from './stores/app.js'
  import { Header, Input, Button, Main, BtnGroup } from 'forui'
  import Order from './Order.svelte'
  import router from 'svelte-router'
  import {
    ActionDone,
    ActionSearch,
    ActionToday
  } from 'svelte-material-icons'
</script>

<style>

</style>
