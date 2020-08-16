<script>
  import { Link } from "svelte-routing";
</script>

<style>
  nav {
    background: black;
    display: flex;
    height: 70px;
    align-items: center;
    justify-content: space-around;
  }

  .section {
    display: flex;
  }

  .brand {
    color: white;
    font-size: 1.5rem;
  }

  .nav-item {
    padding: 0 10px;
    color: white;
  }
</style>

<nav>
  <Link to="/" class="section">
    <div class="brand">Brand</div>
  </Link>
  <div class="section">
    <Link to="/about" class="nav-item">
      <div class="nav-item">About</div>
    </Link>
    <Link to="/demo" class="nav-item">
      <div class="nav-item">Demo</div>
    </Link>
  </div>
</nav>
