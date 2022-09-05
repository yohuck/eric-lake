<header>
    <nav>
        <ul>
            <li>about</li>
            <li>skills</li>
            <li>work</li>
            <li>contact</li>
        </ul>
    </nav>
</header>

<style>
nav{
    width: 100%;
    position: fixed;
}

nav ul{
    max-width: 1500px;
    margin: 0 auto;
    display: flex;
    justify-content: flex-end;
}

li{
    margin: var(--size-2);
    list-style: none;
    color: var(--violet-7);
}

li:hover, li:active{
    border-bottom: dotted var(--violet-7);
}
</style>