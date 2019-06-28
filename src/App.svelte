<Header>
  <h1 slot="left">{app.title}</h1>
  <nav slot="center">
    <Button flat active={tmp === 'a'} on:click={() => (tmp = 'a')}>
      prev
    </Button>
    <Button icon flat active={tmp === 'b'} on:click={() => (tmp = 'b')}>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="24"
        height="24"
        viewBox="0 0 24 24">
        <path d="M0 0h24v24H0z" fill="none" />
        <path
          d="M22 5.72l-4.6-3.86-1.29 1.53 4.6 3.86L22 5.72zM7.88 3.39L6.6 1.86
          2 5.71l1.29 1.53 4.59-3.85zM12.5 8H11v6l4.75
          2.85.75-1.23-4-2.37V8zM12 4c-4.97 0-9 4.03-9 9s4.02 9 9 9c4.97 0
          9-4.03 9-9s-4.03-9-9-9zm0 16c-3.87 0-7-3.13-7-7s3.13-7 7-7 7 3.13 7
          7-3.13 7-7 7z" />
      </svg>
    </Button>
    <Button flat success active={tmp === 'c'} on:click={() => (tmp = 'c')}>
      next
    </Button>
  </nav>
  <nav slot="right">
    <BtnGroup>
      <Button flat icon active={tmp === 'a'} on:click={() => (tmp = 'a')}>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24">
          <path d="M0 0h24v24H0z" fill="none" />
          <path d="M9 16.17L4.83 12l-1.42 1.41L9 19 21 7l-1.41-1.41z" />
        </svg>
      </Button>
      <Button flat icon active={tmp === 'b'} on:click={() => (tmp = 'b')}>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24">
          <path d="M0 0h24v24H0z" fill="none" />
          <path
            d="M22 5.72l-4.6-3.86-1.29 1.53 4.6 3.86L22 5.72zM7.88 3.39L6.6
            1.86 2 5.71l1.29 1.53 4.59-3.85zM12.5 8H11v6l4.75
            2.85.75-1.23-4-2.37V8zM12 4c-4.97 0-9 4.03-9 9s4.02 9 9 9c4.97 0
            9-4.03 9-9s-4.03-9-9-9zm0 16c-3.87 0-7-3.13-7-7s3.13-7 7-7 7 3.13
            7 7-3.13 7-7 7z" />
        </svg>
      </Button>
      <Button flat icon active={tmp === 'c'} on:click={() => (tmp = 'c')}>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24">
          <path d="M12 8V4l8 8-8 8v-4H4V8z" />
          <path d="M0 0h24v24H0z" fill="none" />
        </svg>
      </Button>
    </BtnGroup>
  </nav>
</Header>

<Main>
  <table style="width:100%">
    <tr>
      <th>default</th>
      <th>inverse</th>
      <th>flat</th>
      <th>fl inv</th>
      <th>active</th>
      <th>act inv</th>
      <th>disabled</th>
      <th>dis inv</th>
      <th>icon</th>
      <th>ic inv</th>
      <th>ic fl</th>
    </tr>
    <tr>
      <th>
        <Button>But</Button>
      </th>
      <th>
        <Button inverse>But</Button>
      </th>
      <th>
        <Button flat>But</Button>
      </th>
      <th>
        <Button flat inverse>But</Button>
      </th>
      <th>
        <Button active>But</Button>
      </th>
      <th>
        <Button active inverse>But</Button>
      </th>
      <th>
        <Button disabled>But</Button>
      </th>
      <th>
        <Button disabled inverse>But</Button>
      </th>
      <th>
        <Button icon>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24">
            <path d="M0 0h24v24H0z" fill="none" />
            <path
              d="M22 5.72l-4.6-3.86-1.29 1.53 4.6 3.86L22 5.72zM7.88 3.39L6.6
              1.86 2 5.71l1.29 1.53 4.59-3.85zM12.5 8H11v6l4.75
              2.85.75-1.23-4-2.37V8zM12 4c-4.97 0-9 4.03-9 9s4.02 9 9 9c4.97 0
              9-4.03 9-9s-4.03-9-9-9zm0 16c-3.87 0-7-3.13-7-7s3.13-7 7-7 7
              3.13 7 7-3.13 7-7 7z" />
          </svg>
        </Button>
      </th>
      <th>
        <Button icon inverse>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24">
            <path d="M0 0h24v24H0z" fill="none" />
            <path
              d="M22 5.72l-4.6-3.86-1.29 1.53 4.6 3.86L22 5.72zM7.88 3.39L6.6
              1.86 2 5.71l1.29 1.53 4.59-3.85zM12.5 8H11v6l4.75
              2.85.75-1.23-4-2.37V8zM12 4c-4.97 0-9 4.03-9 9s4.02 9 9 9c4.97 0
              9-4.03 9-9s-4.03-9-9-9zm0 16c-3.87 0-7-3.13-7-7s3.13-7 7-7 7
              3.13 7 7-3.13 7-7 7z" />
          </svg>
        </Button>
      </th>
      <th>
        <Button icon flat>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24">
            <path d="M0 0h24v24H0z" fill="none" />
            <path
              d="M22 5.72l-4.6-3.86-1.29 1.53 4.6 3.86L22 5.72zM7.88 3.39L6.6
              1.86 2 5.71l1.29 1.53 4.59-3.85zM12.5 8H11v6l4.75
              2.85.75-1.23-4-2.37V8zM12 4c-4.97 0-9 4.03-9 9s4.02 9 9 9c4.97 0
              9-4.03 9-9s-4.03-9-9-9zm0 16c-3.87 0-7-3.13-7-7s3.13-7 7-7 7
              3.13 7 7-3.13 7-7 7z" />
          </svg>
        </Button>
      </th>
    </tr>
    <tr>
      <th>
        <Button success>But</Button>
      </th>
      <th>
        <Button inverse success>But</Button>
      </th>
      <th>
        <Button flat success>But</Button>
      </th>
      <th>
        <Button flat inverse success>But</Button>
      </th>
      <th>
        <Button active success>But</Button>
      </th>
      <th>
        <Button active inverse success>But</Button>
      </th>
      <th>
        <Button disabled success>But</Button>
      </th>
      <th>
        <Button disabled inverse success>But</Button>
      </th>
      <th>
        <Button icon success>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24">
            <path d="M0 0h24v24H0z" fill="none" />
            <path
              d="M22 5.72l-4.6-3.86-1.29 1.53 4.6 3.86L22 5.72zM7.88 3.39L6.6
              1.86 2 5.71l1.29 1.53 4.59-3.85zM12.5 8H11v6l4.75
              2.85.75-1.23-4-2.37V8zM12 4c-4.97 0-9 4.03-9 9s4.02 9 9 9c4.97 0
              9-4.03 9-9s-4.03-9-9-9zm0 16c-3.87 0-7-3.13-7-7s3.13-7 7-7 7
              3.13 7 7-3.13 7-7 7z" />
          </svg>
        </Button>
      </th>
      <th>
        <Button icon inverse success>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24">
            <path d="M0 0h24v24H0z" fill="none" />
            <path
              d="M22 5.72l-4.6-3.86-1.29 1.53 4.6 3.86L22 5.72zM7.88 3.39L6.6
              1.86 2 5.71l1.29 1.53 4.59-3.85zM12.5 8H11v6l4.75
              2.85.75-1.23-4-2.37V8zM12 4c-4.97 0-9 4.03-9 9s4.02 9 9 9c4.97 0
              9-4.03 9-9s-4.03-9-9-9zm0 16c-3.87 0-7-3.13-7-7s3.13-7 7-7 7
              3.13 7 7-3.13 7-7 7z" />
          </svg>
        </Button>
      </th>
      <th>
        <Button icon flat success>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24">
            <path d="M0 0h24v24H0z" fill="none" />
            <path
              d="M22 5.72l-4.6-3.86-1.29 1.53 4.6 3.86L22 5.72zM7.88 3.39L6.6
              1.86 2 5.71l1.29 1.53 4.59-3.85zM12.5 8H11v6l4.75
              2.85.75-1.23-4-2.37V8zM12 4c-4.97 0-9 4.03-9 9s4.02 9 9 9c4.97 0
              9-4.03 9-9s-4.03-9-9-9zm0 16c-3.87 0-7-3.13-7-7s3.13-7 7-7 7
              3.13 7 7-3.13 7-7 7z" />
          </svg>
        </Button>
      </th>
    </tr>
    <tr>
      <th>
        <Button danger>But</Button>
      </th>
      <th>
        <Button inverse danger>But</Button>
      </th>
      <th>
        <Button flat danger>But</Button>
      </th>
      <th>
        <Button flat inverse danger>But</Button>
      </th>
      <th>
        <Button active danger>But</Button>
      </th>
      <th>
        <Button active inverse danger>But</Button>
      </th>
      <th>
        <Button disabled danger>But</Button>
      </th>
      <th>
        <Button disabled inverse danger>But</Button>
      </th>
      <th>
        <Button icon danger>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24">
            <path d="M0 0h24v24H0z" fill="none" />
            <path
              d="M22 5.72l-4.6-3.86-1.29 1.53 4.6 3.86L22 5.72zM7.88 3.39L6.6
              1.86 2 5.71l1.29 1.53 4.59-3.85zM12.5 8H11v6l4.75
              2.85.75-1.23-4-2.37V8zM12 4c-4.97 0-9 4.03-9 9s4.02 9 9 9c4.97 0
              9-4.03 9-9s-4.03-9-9-9zm0 16c-3.87 0-7-3.13-7-7s3.13-7 7-7 7
              3.13 7 7-3.13 7-7 7z" />
          </svg>
        </Button>
      </th>
      <th>
        <Button icon inverse danger>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24">
            <path d="M0 0h24v24H0z" fill="none" />
            <path
              d="M22 5.72l-4.6-3.86-1.29 1.53 4.6 3.86L22 5.72zM7.88 3.39L6.6
              1.86 2 5.71l1.29 1.53 4.59-3.85zM12.5 8H11v6l4.75
              2.85.75-1.23-4-2.37V8zM12 4c-4.97 0-9 4.03-9 9s4.02 9 9 9c4.97 0
              9-4.03 9-9s-4.03-9-9-9zm0 16c-3.87 0-7-3.13-7-7s3.13-7 7-7 7
              3.13 7 7-3.13 7-7 7z" />
          </svg>
        </Button>
      </th>
      <th>
        <Button icon flat danger>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24">
            <path d="M0 0h24v24H0z" fill="none" />
            <path
              d="M22 5.72l-4.6-3.86-1.29 1.53 4.6 3.86L22 5.72zM7.88 3.39L6.6
              1.86 2 5.71l1.29 1.53 4.59-3.85zM12.5 8H11v6l4.75
              2.85.75-1.23-4-2.37V8zM12 4c-4.97 0-9 4.03-9 9s4.02 9 9 9c4.97 0
              9-4.03 9-9s-4.03-9-9-9zm0 16c-3.87 0-7-3.13-7-7s3.13-7 7-7 7
              3.13 7 7-3.13 7-7 7z" />
          </svg>
        </Button>
      </th>
    </tr>
  </table>
</Main>

<script>
  import { Header, Button, Main, BtnGroup } from 'forui'

  const app = {
    title: 'Softy club'
  }

  let tmp = ''
</script>

<style>

</style>
