
    <div class="cont">
        <input type="checkbox" id='hide'>
        <label for='hide'>
        <div class="scanner">
        <div class="card">
          <div class="stripe-chip"></div>
          <div class="info">
            <p>Platinum Member</p>
            <p class='digits'>1001 2002 3003 4200</p>
          </div>
        </div>
        </div>
         </label>
    </div>
<!--     <div class="scanner">
    <div class="card gold">
      <div class="stripe"></div>
      <div class="info">
        <p>Gold Memberr</p>
        <p class='digits'>1001 2002 3003 4200</p>
      </div>
    </div> -->
  


  <style>

.cont   {
    display: grid;
    place-items: center;
    padding: var(--size-1);

}



#hide {
  display:none;
}


.scanner {
    margin: var(--size-5);
  /* transform: rotate(90deg); */
  border-left: 10px solid  var(--violet-3);
  /* width: 19rem; */
  overflow: hidden;
  border-radius:2px;
}

.scanner:hover, .scanner:focus {
  cursor: pointer;
}

.card {
  border: 1px solid black;
  height: 8rem;
  width: 12.4rem;
  border-radius: 1rem;
  transition: 0.5s;
  margin: 0.5rem;
  background-color: #1D3557;
  box-shadow: var(--shadow-5);
}

#hide:checked +label .card  {
  transform: translate(-10rem);
}

#hide:checked +label .scanner  {
 border-left: 10px solid var(--lime-8);
 transition-delay: .4s;
}

/* .stripe {
  margin-top: 1.7rem;
  height: 2.2rem;
  width: 14..7rem;
  background-color: black;
} */

.info {
  margin-top: 1rem;

  text-align: center;
  color: #848FA5;
  text-shadow: -1px -1px 1px #fff, 1px 1px 1px #000;
  letter-spacing: .12rem;
}

.info .digits {
  letter-spacing: .2rem;
}

.stripe-chip {
  margin-top: 1rem;
  margin-left: 1rem;
  margin-bottom: 1.3rem;
  height: 2rem;
  width: 2.6rem;
  border-radius: 0.5rem;
  background-color: #e4eee9;
background-image: linear-gradient(315deg, #5b47ce 0%, #93a5ce 74%);

}

p{
    font-size: 0.6rem;
}

  </style>