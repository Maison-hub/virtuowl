<script>

</script>

<template>
<footer>
    <div class="title">Nos RESEAUX 🚀</div>

    <div class="rs">
        <a href="https://www.youtube.com/channel/UC6hz5XTZE2QkGsolAwCr88Q">
            <img src="/_nuxt/assets/images//rs/youtube.svg" alt="youtube">
        </a>
        <a href="https://www.linkedin.com/company/103465534/admin/feed/posts/?feedType=following">
            <img src="/_nuxt/assets/images//rs/linkedin.svg" alt="linkedin">
        </a>
        <a href="https://www.instagram.com/virtuowl.ncy/">
            <img src="/_nuxt/assets/images//rs/youtube.svg" alt="insta">
        </a>
    </div>
    <p>
        made with ❤️ par <a href="https://github.com/Maison-hub?tab=repositories" target="_blank">maison-hub</a>
    </p>
</footer>
</template>

<style>
footer{
    position: relative;
    background-color: var(--blue);
    z-index: 100;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    padding: 5vw;
    gap: 24px;
}

footer .title{
    -webkit-text-stroke: 1px var(--white);
    font-size: 6vw !important;
    color: transparent;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
}

.rs{
    display: flex;
    align-items: center;
    justify-content: flex-end;
    gap: 24px;
    width: 100%;

}

.rs a img{
    height: 10vh;
}

</style>