<div id="header">
    <img class='left' src="../rbolobo_wh_cl.svg" style="width: 20vw" alt="logo">
    <div class='right tall'>
        <a href="/">Home</a>
        <a href="/competition">Competitions</a>
        <a href="/robots">Robots</a>
        <a href="/#sponsors">Sponsors</a>
        <a href="https://github.com/frc2359" target="_blank" style='display:flex'><img style='align-self:center' src="../github-mark-white.png" alt='Github Logo'></a>
    </div>
</div>

<style>
#header {
        padding-left: 0px;
        z-index: 999;
        backdrop-filter: invert(10%) blur(9px);
        position: fixed;
        background-image: var(--gray-200-glass);
        width: 100vw;
        display: grid;
        grid-template-columns: 20vw 80vw;
        align-items: center;
        justify-content: center;
        height: 12vh;
        top: 0;
        margin-top: 0;
        margin-bottom: 0;
        padding-top: 0;    
        padding-bottom: 0;  
        border-radius: 0px 0px 20px 20px;  
    }
    .left {
        align-self: center;
        margin-top: 0vh;
        margin-bottom: 0vh;
        padding-left: 2vw;
        font-size: 2vh;
        width: 60vw;
        font-weight: 600;
        
    }
    .right {
        display: flex;
        margin-right: 5vw;
        justify-self: end;
        align-items: center;
        justify-content: center;
        flex-direction: row;
    }
    .right a {
        display: block;
		font-family: 'Rockwell', 'Arvo', 'sans-serif';
        color: var(--green-300);
        align-self: center;
        font-size: 4vh;
        text-decoration: none;
        margin: 0;
        padding: 0;
        padding-left: 2vw;
        transition: ease .7s;
    }
    .right a img {
        max-width: 2vw;
        filter: brightness(80%);
        transition: ease .7s;
    }
    .right a img:hover {
        filter: brightness(50%);
        transition: cubic-bezier(.57,-0.01,0,.72) 200ms;
    }
    .right a:hover {
        color: var(--green-200);
        transition: cubic-bezier(.57,-0.01,0,.72) 200ms;
    }
</style>