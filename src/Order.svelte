<Button danger on:click={() => router.go({ branch: 'order' })}>
  branch_order
</Button>
<Button success on:click={() => router.go({ branch: 'fabric' })}>
  branch_fabric
</Button>
<br />
<br />
<Button success inverse on:click={() => router.go({ action: 'index' })}>
  action_index
</Button>
<Button danger inverse on:click={() => router.go({ action: 'view' })}>
  action_view
</Button>
<br />
<br />
<Button inverse on:click={() => router.go({ page: 1 })}>page_1</Button>
<Button flat on:click={() => router.go({ page: null })}>page_null</Button>
<br />
<br />
<Button on:click={() => router.go({ id: 1 })}>id_1</Button>
<Button on:click={() => router.go({ id: null })}>id_null</Button>
<br />
<br />
<Input
  on:change={e => router.go({ query: e.detail })}
  value={$router.query}
  label="query"
  type="date" />
<Input
  on:input={e => router.go({ query: e.detail })}
  value={$router.search}
  label="query"
  valid
  type="number" />
<Input
  on:input={e => router.go({ query: e.detail })}
  value={$router.query}
  label="query"
  error
  type="text" />
<Button on:click={() => router.go({ query: null })}>reset</Button>
<br />
<br />
<a href="/order/view?id=123">order_123</a>
<a href="/order/index?query=123">orders_query</a>
<a href="/order/index?query=(a:1, b:2)">orders_query</a>

<script>
  import router from 'svelte-router'
  import { Button, Input } from 'forui'
</script>

<style type="scss">
  :global(button) {
    background: cp(10%, 10%) !important;
  }
</style>
