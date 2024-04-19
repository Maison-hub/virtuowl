<script setup>
const props = defineProps({
    link: String,
    description: String,
    image: String
})
</script>


<template>

    <div class="projectCard">
        <a :href="$props.link" target="_blank">
            <img class="projectCard_img" :src="$props.image" :style="{ backgroundSize: 'contain', backgroundPosition: 'center', backgroundRepeat: 'no-repeat' }"/>
        
        </a>
        
        <div class="projectCard_content">
            <p class="projectCard_description">{{ $props.description }}</p>
        </div>
    </div>
</template>

<style>
.projectCard{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 100%;
    background-color: var(--blue);
    color: var(--white);
    padding: 32px 24vw;
    margin: 24px 0;
    gap: 32px;
}
.projectCard_img{
    border-radius: 12px;
    width: 50vw;
    transition: box-shadow .2s ease-in-out;
}

.projectCard_img:hover{
    box-shadow: 0px 0px 40px 8px #fffbf255; 
}

.projectCard_content{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 50vw;
    gap: 22px;
}

.projectCard_description{
    font-size: 18px;
    font-weight: 500;
    line-height: 1.5;
}
</style>