<script>
  export var audio = new Audio("CLE_Reverse_Fx_5.wav");
  console.log(audio);
  function playsound(){
    audio.play();
  }

</script>

<button on:click={playsound}>
    play
  </button>

  <style>
button{
    background-color: rebeccapurple;
  }
  </style>