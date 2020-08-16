<script>
  let loading = false;
  let users = [];

  const onGetUsers = async () => {
    loading = true;
    const data = await fetch("http://api.github.com/users");
    if (data.ok) {
      users = await data.json();
      loading = false;
    }
  };

  onGetUsers();
</script>

<div>
  <div>
    <h1>Demo</h1>
  </div>

  {#if loading}
    <div>Loading</div>
  {:else}
    <ul>
      {#each users as user}
        <li>{user.login}</li>
      {/each}
    </ul>
  {/if}

</div>
