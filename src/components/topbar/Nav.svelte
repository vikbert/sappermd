<script>
  export let segment;
</script>

<style>
  .navigation {
    display: flex;
    justify-content: flex-end;
    padding-right: 2rem;
  }
  ul {
    margin: 0;
    padding: 0;
  }

  ul::after {
    content: '';
    display: block;
    clear: both;
  }

  li {
    display: block;
    float: left;
    margin-bottom: 0.2rem;
  }

  .selected {
    position: relative;
    display: inline-block;
  }

  .selected::after {
    position: absolute;
    content: '';
    width: calc(100% - 1em);
    height: 2px;
    display: block;
  }

  a {
    text-decoration: none;
    padding: 0.5em 0.5em;
    display: block;
  }
</style>

<div class="navigation">
  <ul>
    <li><a class:selected={segment === undefined} href=".">Home</a></li>
    <li><a class:selected={segment === 'about'} href="about">About</a></li>
  </ul>
</div>
