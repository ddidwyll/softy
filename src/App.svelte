<Header>
  <h1 slot="left">{title}</h1>
  <nav slot="right">
    <BtnGroup>
      <Button icon active={$tmp === 'a'} on:click={() => ($tmp = 'a')}>
        <ActionToday />
      </Button>
      <Button icon active={$tmp === 'b'} on:click={() => ($tmp = 'b')}>
        <ActionVisibility />
      </Button>
      <Button icon active={$tmp === 'c'} on:click={() => ($tmp = 'c')}>
        <ActionVisibilityOff />
      </Button>
    </BtnGroup>
  </nav>
</Header>

<Main>
  <ActionDone />
  <ActionSearch />
  <ActionToday />
  <pre>{JSON.stringify($router, null, 2)}</pre>
  <a href="#main?id=12345">main_123</a>
  <a href="#main">main</a>
  <a href="#orders?view=1234">orders_1234</a>
  <a href="#orders">orders</a>
</Main>

<script>
  import { tmp, title } from './stores/app.js'
  import { Header, Button, Main, BtnGroup } from 'forui'
  import router from 'svelte-router'
  import {
    ActionDone,
    ActionSearch,
    ActionToday,
    ActionVisibility,
    ActionVisibilityOff
  } from 'svelte-material-icons'
</script>

<style>

</style>
