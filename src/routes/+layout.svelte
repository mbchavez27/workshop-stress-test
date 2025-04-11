<header>
  <div>
    <h1>Sample LEAP Workshop</h1>
  </div>
  <div class="orgTitle">
    <h1>LSCS</h1>
  </div>
</header>

<slot></slot>

<style>
  header {
    background-color: #d0273b;
    color: white;
    padding: 1.5em 3em;
    display: flex;
    justify-content: space-between;
  }
  header > div > h1 {
    font-weight: bold;
    font-size: 2em;
  }

  .orgTitle {
    padding-right: 2.5em;
  }
</style>
