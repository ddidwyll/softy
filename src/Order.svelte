<Input
  value={$router.query}
  on:input={e => router.go({ query: e.detail || null })}
  label="Olololol" />
<Button label="ok" />
<Button label="cancel" />
<br />
<br />
<Input
  value={$router.query}
  on:input={e => router.go({ query: e.detail || null })}
  type="number"
  valid>
  <ActionDone hidden={$router.query === "ok"} />
</Input>
<br />
<br />
<Input
  value={$router.query}
  on:input={e => router.go({ query: e.detail || null })}
  type="search"
  disabled >
  <ActionToday />
</Input>
<br />
<br />
<Input
  value={$router.query}
  on:input={e => router.go({ query: e.detail || null })}
  type="date">
  <Button label="go"/>
</Input>
<br />
<br />
<Input
  clean
  value={$router.query}
  on:input={e => router.go({ query: e.detail || null })}
  label="Search">
  <ActionSearch />
</Input>

<script>
  import router from 'svelte-router'
  import { Input, Button } from 'forui'
  import {
    ActionDone,
    ActionSearch,
    ActionToday
  } from 'svelte-material-icons'
</script>
