<script>
  const name = "dog";
  const channel = "<b>sajbox</b>";
  const hack = '<a href="#" onclick="alert(\'hacked\')">click me</a>';
  const id = "heading";
  const disabled = false;
  const status = "success";
  const promoted = true;
</script>

<main>
  <h2 class="underline">underline</h2>
  <h2 class={status}>status</h2>
  <h2 class:promoted>Movie Title</h2>

  <h1>hello {name}</h1>
  <div>{@html channel}</div>
  <div>{@html hack}</div>
  <h2 {id}>heading</h2>
  <button {disabled}>disabled</button>
</main>

<style>
  .underline {
    text-decoration: underline;
  }

  .danger {
    color: red;
  }

  .success {
    color: green;
  }

  .promoted {
    font-style: italic;
  }

  main {
    text-align: center;
    max-width: 240px;
    padding: 1em;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

