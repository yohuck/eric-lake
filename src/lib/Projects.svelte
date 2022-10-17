<script>
import Popper from "./popper.svelte";
import Card from "./Card.svelte"

</script>
<!-- <section class="backdrop title">
    <h2>Check out my work:<br><span></span></h2>
</section> -->
<div class="con">
    
    <section class="backdrop">
        <article >
            <div class="info">
                <div class="top">
                    <h4>Talking Cents</h4>
                    <hr>
                    <div class="grp">
                        <a href="https://github.com/yohuck/daily-chatter" target="_blank">GitHub Repo</a>
                        <a href="https://talking-cents.com/" target="_blank">Live Site</a>
                    </div>
                    <p>Talking Cents is a social platform that puts your opinions to the test to see how much sense (cents) you really make..</p>
                </div>
                <ul>
                    <li>RedwoodJs</li>
                    <li>React</li>
                    <li>TailwindCSS</li>
                    <li>PostgreSQL</li>
                    <li>GraphQL</li>
                    <li>Prisma</li>
                </ul>
            </div>
        </article>
        <article >
            <div class="info">
                <div class="top">
                    <h4>Habit Stack</h4>
                    <hr>
                    <div class="grp">
                        <a href="https://github.com/yohuck/habit-map" target="_blank">GitHub Repo</a>
                        <a href="https://habitstack.herokuapp.com/" target="_blank">Live Site</a>
                    </div>
                    <p>A full stack application that helps build habit that stick through repetition and reward.</p>
                </div>
                <ul>
                    <li>MySql</li>
                    <li>Express</li>
                    <li>Handlebars</li>
                    <li>Sequelize</li>
                    <li>Node.js</li>
                    <li>Authentication</li>
                </ul>
            </div>
        </article>

        <!-- <article >
            <div class="info">
                <div class="top">
                    <h4>React Portfolio</h4>
                    <hr>
                    <div class="grp">
                        <a href="https://github.com/yohuck/react-portfolio" target="_blank">GitHub Repo</a>
                        <a href="https://react-portfolio-yohuck.vercel.app/" target="_blank">Live Site</a>
                    </div>
                    <p>It's pretty much the same portfolio, but built in React!</p>
                </div>
                <ul>
                    <li>React</li>
                    <li>OpenProps</li>
                    <li>EmailJs</li>
                </ul>
            </div>
        </article> -->
        <article>
            <div class="info">
                <div class="top">
                    <h4>API Resume</h4>
                    <hr>
                    <div class="grp">
                        <a target='blank' href="https://github.com/yohuck/api-resume">GitHub Repo</a>
                        <a target="blank" href="https://eric-lake-api-resume.vercel.app/">Live Site</a>
                    </div>
                    <p>Check out my docs, then fetch my resume as a REST API</p>
                </div>
                <ul>
                    <li>MongoDB</li>
                    <li>Mongoose</li>
                    <li>AWS Cluster</li>
                    <li>Vercel + Serverless Functions</li>
                    <li>Node.js</li>
                </ul>
            </div>
        </article>
        <article>
            <div class="info">
                <div class="top">
                    <h4>Recycle Better</h4>
                    <hr>
                    <div class="grp">
                        <a target='blank' href="https://github.com/yohuck/wish-cycle">GitHub Repo</a>
                        <a target="blank" href="https://yohuck.github.io/wish-cycle/">Live Site</a>
                    </div>
                    <p>A web application to help conscious consumers quickly and easily find the best way to recycle or dispose of household items.</p>
                </div>
                <div class="btm">
    
                    <ul>
                        <li>JQuery</li>
                        <li>Socrata Open API</li>
                        <li>Geolocation API</li>
                        <li>Bulma</li>
                        <li>JavaScript</li>
                    </ul>
                    <!-- <img src="../src/assets/a.gif" alt=""> -->
                            </div>
                </div>
        </article>
        <article>
            <div class="info">
                <div class="top">
                    <h4>City Weather</h4>
                    <hr>
                    <div class="grp">
                        <a target='blank' href="https://github.com/yohuck/city-weather">GitHub Repo</a>
                        <a target="blank" href="https://yohuck.github.io/city-weather/">Live Site</a>
                    </div>
                    <p>A web application using the OpenWeather API to find and store weather information.</p>
                </div>
                <ul>
                    <li>OpenWeather API</li>
                    <li>JavaScript</li>
                    <li>CSS3</li>
                    <li>HTML5</li>
                </ul>
            </div>
        </article>
        <article class="card">
            <div class="top">
                <div class="info">
                    <h4>Chip Card Button</h4>
                    <hr>
                    <div class="grp">
                        <a target='blank' href="https://codepen.io/yohuck/pen/dyJZXxQ">CodePen</a>
                    </div>
                </div>
            </div>
            <Card />
        </article>
        
        <article class="pop">
            <div class="top">
                <div class="info">
                    <h4>Popper Toy</h4>
                    <hr>
                    <div class="grp">
                        <a target='blank' href="https://codepen.io/yohuck/pen/bGaLKaW">Codepen</a>
                    </div>
                </div>
            </div>
            <Popper />
        </article>
        <article>
            <div class="info">
                <div class="top">
                    <h4>Contact Me</h4>
                    <hr>
                    <p>Let's connect! I'm currently open to full time and freelance projects remotely and in the Denver, CO area.</p>
                </div>
                <ul>
                    <a href="https://github.com/yohuck" target="_blank">
                        <li><i class="fa-brands fa-github fa-lg clr keyf" alt="github"></i></li>
                    </a>
                    <a href="https://linkedin.com/in/eric-lake" target="_blank">
                    <li><i class="fa-brands fa-linkedin fa-lg clr keyf" alt="linkedin"></i></li>
                    </a>
                    <a href="mailto:ericallenlake@gmail.com" target="_blank">
                    <li><i class="fa-duotone fa-envelope fa-lg clr keyf" alt="email"></i></li>
                        </a>
                        <a href="https://twitter.com/itsyohuck" target="_blank">
                    <li><i class="fa-brands fa-twitter fa-lg clr keyf" alt="twitter"></i></li>
                    </a>
                </ul>
            </div>
        </article>
    

    
    
    
    </section>
</div>

<style>
    @import "open-props/colors-hsl";
*{
    box-sizing: border-box;
    /* border: 1px solid red; */
}

ul a li i:hover{
    color: var(--indigo-1)
}
ul a li i{
    padding: var(--size-2);
}
ul a li{
    margin-top: var(--size-8);
}

.con{
    background-color: hsl(var(--indigo-9-hsl) / 100%);
}
    .pop{
        display: flex;
        justify-content: center;
        flex-direction: column;
        justify-content: space-between;
    }

    .btm{
        display: flex;
        justify-content: center;
        align-items: flex-end;
    }


    .card, .pop{
        display: flex;
        flex-direction: column;
        justify-content: space-between;

    }

    article{
        /* aspect-ratio: 1; */
    }



.backdrop {
  background-color: hsl(var(--indigo-9-hsl) / 90%);
}

    section{
        background-color: hsl(var(--gray-3-hsl) / 30%);
        background-size: 3000px 3000px;
        margin: 0;
        /* overflow: auto; */
        padding: var(--size-3);
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
        /* grid-auto-columns: minmax(300px,1fr);
        grid-auto-flow: column; */
        gap: var(--size-2);
    }

    hr{
       background-color: var(--indigo-4);
       height: 3px;
       border-radius: var(--border-size-3);
    }


    p{

        color: var(--gray-1);
        padding: var(--size-1);
        border-radius: var(--border-size-3);
    }

    hr{
        margin: 1rem 0;
    }

    article{
        /* background-image: var(--gradient-8); */
        background-color: black;
        /* height: 100%; */
        /* border: 1px solid black; */
        border-radius: var(--radius-conditional-3);
        padding: var(--size-3);
        box-shadow: var(--shadow-3);
        margin: 0;
        border: var(--border-size-3) solid transparent;
        color: var(--violet-2);
       
        /* max-width: 2fr; */
    }

    h2{ 
        margin: 0;
        padding: 0;
        /* width: 100%; */
        color: var(--indigo-2);
        background-color: black;
        border-radius: var(--radius-conditional-3);
        padding: var(--size-2);
        box-shadow: var(--shadow-3);
        border: var(--border-size-3) solid transparent;

        /* -webkit-background-clip: text;
  -webkit-text-fill-color: transparent; */
    }

    span{
        font-size: var(--font-size-2);
    }

    h4{
        color: var(--indigo-2);
    }

    a{
        margin: 0;
        padding: 0;
    }


    ul{
        width: 100%;
        flex-wrap: wrap;
        margin: 0;
        padding: 0;
        display: flex;
        gap: var(--size-1);
    }

    ul li{
        color: white;
        list-style: none;
        padding: var(--size-1);
        background-color: var(--indigo-6);
        border-radius: var(--border-size-3);
    }



    .info{
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }
</style>