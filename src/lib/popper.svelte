<section>
    <audio  class='audio' id="pop" src="https://assets.codepen.io/7784266/sfx-pop5.mp3"></audio>
  <!--   audio. from https://www.fiftysounds.com/royalty-free-music/sfx-pop5.html -->
    <div class="outer">
      <div class="row">
        <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
      </div>
      <div class="row">
       <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
       
        
      </div>
      <div class="row">
       <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
      </div>
      <div class="row">
       <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>   
      </div>
      <div class="row">
     <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
      </div>
      <div class="row final">
       <div class="popper">
        </div>
        <div class="popper">
        </div>
        <div class="popper">
        </div>
      </div>
    </div>
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

.active {
background: radial-gradient(#442ce0, #31b74a 82%);
  box-shadow: inset 0px 0px 2px rgba(0,0,0,0.3);
  filter:none;
  opacity: 0.75;
}
</style>