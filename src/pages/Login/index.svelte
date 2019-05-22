<script>
  import { push } from "svelte-spa-router";
</script>

<style>
  .container {
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background: #614ea1;
    color: #fff;
    /* background-image: url(http://svite-league-apps-content.s3.amazonaws.com/bgimages/metal.jpg); */
    /* background-repeat: repeat-x; */
    /* background-position: center top; */
  }

  .group {
    padding: 5px;
  }
</style>

<div class="container">
  <div class="group">
    <label for="username">Username:</label>
    <input id="username" name="username" type="text" />
  </div>
  <div class="group">
    <label for="password">Password:</label>
    <input id="password" name="password" type="password" />
  </div>
  <button on:click={() => push('/dactools')}>Login</button>
</div>
