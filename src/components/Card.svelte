<script>
    export let image = '../images/IMG_8009.JPG';
    export let name = 'Tikolai Nesla Fourteenth IV';
    export let year = "Rapid React";
    export let accolades = 'Experience :)';
</script>

<div class="main">
<h1>{name}</h1>
<span>{year}</span>
<img src="{image}" alt="">
<p><b>Accolades:</b><br>
    {@html accolades}
</p>
</div>

<style>
    .main {
        background-color: #474747;
        height: 50vh;
        width: 20vw;
        border-radius: 20px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .main h1 {
        font-size: 3vh;
        margin-bottom: 0px;
        padding-bottom: 0px;
    }
    .main span {
        margin-bottom: 1vh;
    }
    .main img {
        width: 95%;
        height: 50%;
        object-fit: cover;
        object-position: center;
        border-radius: 10px;
    }
    .main p {
        width: 90%;
        height: 10%;
    }
</style>