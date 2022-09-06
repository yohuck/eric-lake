
<section>
   
    <article>
        <div class="info">
        <h4>Habit Stack</h4>
        <hr>
           <div class="grp">
               <a href="github.com">GitHub Repo</a>
               
               <a href="github.com">Live Site</a>
           </div>
        </div>
        <!-- <img src="../src/assets/a.gif" alt=""> -->

    </article>
    <article>
        <h4>Recycle Better</h4>
        <div class="grp">
            <a target='blank' href="https://github.com/yohuck/wish-cycle">GitHub Repo</a>
        
            <a target="blank" href="https://yohuck.github.io/wish-cycle/">Live Site</a>
        </div>
        <!-- <img src="../src/assets/c.gif" alt=""> -->
    </article>
    <article>
        <h4>City Weather</h4>
        <div class="grp">
            <a href="github.com">GitHub Repo</a>
            <a href="github.com">Live Site</a>
        </div>
        <!-- <div class="photo"><img src="../src/assets/b.gif" alt=""></div> -->
    </article>
</section>

<style>
    section{
        background-color: var(--violet-7);
        background-size: cover;
        padding: var(--size-3);
        width: 100%;
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 2fr));
        grid-gap: var(--size-2);
    }

    .info{
    }

    hr{
        margin: 1rem 0;
    }

    article{
        background-image: var(--gradient-8);
        border: 1px solid black;
        border-radius: var(--radius-conditional-3);
        padding: var(--size-3);
        box-shadow: var(--shadow-3);
        border: var(--border-size-3) solid var(--violet-7);
        color: var(--violet-2);
        /* max-width: 2fr; */
    }

    h1{ 
        margin: 0;
        padding: 0;
        width: 100%;
        text-align: center;
    }

    h4{
        color: var(--violet-2);
    }

    a{
        margin: 0;
        padding: 0;
    }

    .grp{
        padding: 2px solid red;
        margin: 0;
    }



    article:hover, article:focus{
        border: var(--border-size-3) solid var(--red-6 );              
        box-shadow: var(--shadow-4);
    }

    .photo{
        display: flex;
    }

    img{
        width: 100%;

    }
</style>