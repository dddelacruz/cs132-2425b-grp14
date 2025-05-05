<script>
    export let avatar;
    export let name;
    export let desc;
    export let link;
</script>

<div class='about-card'>
    <div class='avatar-box'>
        <img class='avatar' src={avatar} alt='avatar'>
    </div>

    <div class='name-box'>
        <p class="name">{name}</p>
    </div>

    <div class='desc-box'>
        <p class="desc">{desc}</p>
    </div>

    <div class='link-box'>
        <p class="link"><a href={link}>Github link</a></p>
    </div>
</div>

<style>
    p{
        margin: 0;
    }

    .name{
        font-weight: bold;
    }

    .name-box{
        height: 10%;
    }

    .desc-box {
        height: 30%;
        padding: 5%;
    }

    .link-box {
        height: 10%;
    }

    .about-card{
        border: 2px solid gray;
        border-radius: 5px;
        height: 400px;
        background-color: white;
        margin: 20px auto;
        width: 300px;
    }

    .avatar-box{
        height: 40%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .avatar {
        border-radius: 50%;
        height: 60%;
    }
</style>