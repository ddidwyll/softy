<Header>
  <h1 slot="left">{title}</h1>
  <div slot="center">
    <Input
      simple
      on:input={e => router.go({ query: e.detail || null })}
      value={$router.query}
      label="Search"
      valid={$router.query === 'cheat'}
      error={$router.query === 'error'}
      clean />
  </div>
  <nav slot="right">
    <BtnGroup>
      <Button
        clean
        active={$tmp === 'a'}
        label="today"
        on:click={() => ($tmp = 'a')}>
        <ActionToday />
      </Button>
      <Button
        small
        clean
        active={$tmp === 'b'}
        on:click={() => ($tmp = 'b')}>
        <ActionDone />
      </Button>
      <Button
        small
        clean
        active={$tmp === 'c'}
        on:click={() => ($tmp = 'c')}>
        <ActionSearch />
      </Button>
      <Button
        small
        clean
        disabled
        active={$tmp === 'c'}
        on:click={() => ($tmp = 'c')}>
        <ActionSearch />
      </Button>
    </BtnGroup>
  </nav>
</Header>

<Main>
  <!--<pre>$router: {JSON.stringify($router, null, 2)}</pre>-->
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
