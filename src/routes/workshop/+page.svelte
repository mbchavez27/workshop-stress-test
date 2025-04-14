<script>
  import '../../global.css'
  let registered = 0
  let isActive = true
  let closed = false

  $: {
    if (registered >= 5) {
      closed = true
      isActive = false
    }
  }

  const register = () => {
    if (!closed) {
      isActive = !isActive
      window.open(
        'https://docs.google.com/forms/d/e/1FAIpQLScgksP_Clr_jtIRtiE8z1Y5c4OiTxTaERh9tAEGlisNEFSkHg/viewform?usp=dialog',
      )
      registered++
      setTimeout(() => {
        isActive = !isActive
      }, 3000)
    }
  }
</script>

<div>
  <span>
    <h2>Sample Workshop #1</h2>
    <p class={closed ? '' : 'hide'}>Closed</p>
  </span>
  <p>Workshop Title: Stress testing...</p>
  <p>Number of Registered Students: {registered}</p>
  <button
    on:click={register}
    disabled={!isActive}
    class={`${isActive ? '' : 'inActive'} ${closed ? 'inActive' : ''}`}
    >Register</button
  >
</div>

<style>
  span {
    display: flex;
    gap: 1em;
    margin-bottom: 1em;
  }
  div {
    padding: 1.5em;
    font-size: 1.4em;
  }

  .hide {
    display: none;
  }
  span > p {
    margin-top: 0.3em;
    background-color: #d0273b;
    color: white;
    border-radius: 1em;
    padding: 0.2em;
    font-size: 1em;
  }

  div > p {
    margin-top: 0.4em;
    font-size: 1.2em;
  }

  .inActive {
    background-color: gray;
  }
  div > button {
    background-color: #d0273b;
    color: white;
    padding: 1em 2em;
    border-radius: 0.2em;
    margin-top: 1em;
    outline: none;
    border: none;
  }
</style>
