<header>
    <nav>
        <ul>
            <li>About</li>
            <li>Work</li>
            <li>Stack</li>
            <li>Contact</li>
        </ul>
    </nav>
</header>

<style>

nav{
    background-image: var(--gradient-2);
    background-size: 3000px 3000px;
    filter: var(--noise-filter-2);
    width: 100%;
    position: fixed;
    z-index: 10000;
    animation: grad 20s linear 0s infinite alternate none;
}

nav ul{
    text-align: center;
    padding: var(--size-1);
    margin: var(--size-1);
    max-width: 1500px;
    display: flex;
    gap: 1rem;
    justify-content: flex-end;
}

li{
    margin: 0;
    padding: var(--size-1);
    font-weight: var(--font-weight-8);
    /* margin: var(--size-2); */
    list-style: none;
    color: var(--indigo-3);
    border-bottom: 4px dotted transparent;
}

li:hover, li:active{
    border-bottom: 4px dotted var(--indigo-5);
}


@keyframes grad{
    0% {
        background-position: -1000px -2000px;
    }
    22% {
    }
    47% {

    }
    76% {
    }
    100% {
        background-position: 0px 0px;
    }
}
</style>