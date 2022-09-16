
<script>

  let time= 0;
  let paused=true

  const pop = (e) => {
    console.log(e.target.classList)
    paused= false
    time = 0
    if (e.target.classList.contains('active')){
      e.target.classList.remove('active');
//            
          } else {
           e.target.classList.add('active');
//                  
        }
  }



  // creates an array of all the poppers
// let switches = document.querySelectorAll('.popper');
   

//    // initializes the audio
//    let audio = document.getElementById('pop');
   
//    // adds event listeners to all the poppers
//    for (var i = 0; i < switches.length; i++){
//        switches[i].addEventListener('click', function(e){
//          // adds/removed active class & plays audio then sets time = zero so audio can play again.
//           if (this.classList.contains('active')){
//              this.classList.remove('active');
//              audio.currentTime = 0;
//              audio.play();
//              audio.currentTime = 0;
//           } else {
//              this.classList.add('active');
//              audio.currentTime = 0;
//              audio.play();
//              audio.currentTime = 0;        
//           }
//        })
//    };
   
</script>


<section>
    <audio  
    class='audio' 
    id="pop" 
    src="https://assets.codepen.io/7784266/sfx-pop5.mp3"
    bind:currentTime={time}
    bind:paused>
  </audio>
  <!--   audio. from https://www.fiftysounds.com/royalty-free-music/sfx-pop5.html -->
    <div class="outer">
      <div class="row">
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
      </div>
      <div class="row">
       <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
       
        
      </div>
      <div class="row">
       <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
      </div>
      <div class="row">
       <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>   
      </div>
      <div class="row">
     <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
      </div>
      <div class="row final">
       <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
        <div class="popper" on:click={pop}>
        </div>
      </div>
    </div>
    <div class="hr active"></div>
</section>

<style>
    section{

        display: flex;
  justify-content: center;
  align-items: center;
    }

    
.outer {
    margin: var(--size-5);
  border: 5px solid var(--grape-6);
  background-color: #efd002;
  background-image: var(--gradient-2);
  padding:0.5rem;
  border-radius: 999px;
  overflow: hidden;
  filter: drop-shadow(0px 0px 1rem black);
  opacity: 100%;
}

.row {
  display: flex;
  justify-content: center;
  align-items: center;
}


.popper {
  width: 1.4rem;
  height: 1.4rem;
  margin: 0.1rem;
  background: var(--gradient-2);
  border-radius: 999px;
  display: flex;
  align-items: center;
  justify-content: center;
  filter: drop-shadow(0px 0px 1rem #31b74a);
  cursor: pointer;
}

.active{
  background: var(--gradient-11);
  filter: drop-shadow(0px 0px 2rem #a425a2);
}



</style>