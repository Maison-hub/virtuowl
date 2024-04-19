<script setup>
const props = defineProps(['name', 'description', 'quote', 'image'])

</script>

<template>

<div class="teamCard">
    <div class="teamCard_img" :style="{ backgroundImage: `url(${image})`, backgroundSize: 'cover', backgroundPosition: 'center', backgroundRepeat: 'no-repeat' }">
        <div class="description">
            <p>{{$props.description}}</p>
        </div>
    </div>
    <div class="teamCard_content">
        <p class="quote">{{$props.quote}}</p>
        <p class="name">{{$props.name}}</p>

    </div>
</div>

</template>

<style>
.teamCard_img{
    height: 35vh;
    width: 18vw;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-end;
}

.description{
    height: 60%;
    width: 100%;
    background-color: var(--blue);
    padding: 18px;
    background: rgb(11,19,43);
    background: linear-gradient(0deg, rgba(11,19,43,1) 0%, rgba(11,19,43,0) 100%);
    color: var(--white);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-end;
    font-weight: 700;
}

.quote{
    font-size: 18px;
    font-weight: 700;
    color: var(--secondary-blue);
}
.quote::before{
    content: '"';
}
.quote::after{
    content: '"';
}
.teamCard_content{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
</style>