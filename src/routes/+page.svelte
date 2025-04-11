<script>
  import "../global.css";
</script>

<div class="page">
  <div class="workshop">
    <h1>This is a Sample Workshop!</h1>
    <p>Register here!</p>
    <a href="/workshop">Workshop</a>
  </div>
</div>

<style>
  .workshop {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 1em;
    padding-top: 8em;
  }

  .workshop > h1 {
    font-size: 2.8em;
  }

  .workshop > p {
    font-size: 1.5em;
  }

  .workshop > a {
    background-color: #d0273b;
    color: white;
    padding: 1em 2em;
    border-radius: 0.2em;
    margin-top: 0.5em;
    outline: none;
    font-size: 1em;
  }
</style>
