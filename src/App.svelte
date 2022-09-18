<script>
  import devLogo from './assets/dev-logo.svg'
  import Counter from './lib/Counter.svelte'
  var audio = new Audio("CLE_Reverse_Fx_5.wav");
  console.log(audio);
  function playsound(){
    audio.play();
  }
</script>

<main>
  <div>
    <a href="https://acmcsuf.com" target="_blank"> 
      <img src={devLogo} class="logo dev" alt="Svelte Logo" />
    </a>
  </div>
  <h1>Pachuco's Sound Website</h1>

  <div class="card">
    <Counter />
  </div>
  <button on:click={playsound}>
    play
  </button>
</main>

<style>
  .logo {
    height: em;
    padding: 1.5em;
    will-change: filter;
  }
  
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }

  .logo.dev:hover {
    filter: drop-shadow(0 0 2em #1E6CFF);
  }
  button{
    background-color: rebeccapurple;
  }
</style>
