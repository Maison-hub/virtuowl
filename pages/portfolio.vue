<template>
    <navbar/>

    <div class="w100 p-relative toppart">
        <div class="title stroke p-absolute">
            Portfolio
        </div>
        <h1 class="title">
            Portfolio               
        </h1>
    </div>

    <div class="subtitle">
        <p>
            Voici certains des projets que nous avons pu réaliser depuis notre ouverture. 
        </p>
    </div>

    <div>
        <projectcard 
        link="https://youtu.be/r-PwSkPxC24"
        description="Ce Projet s’est déroulé en décembre 2021.
        Nous avons collaboré avec Pass culture, l’objectif était de montrer que l’accessiblité  la culture à tous est possible.  "
        image="/_nuxt/assets/images/projects/culture-pour-tous.png"
        />

        <projectcard 
        link="https://youtu.be/QwJ4-X5ZmbU"
        description="Ce projet s’est déroulé en mars 2021
        Nous avons collaboré avec le studio Normalprod pour produire un Teaser d'un jeux-vidéo fictif dans le cadre de la R305 Stratégies de communication et marketing 2023.  Réalisé par ADAM Corentin, ADAM Nils, BOSTOEN Valentin et METZGER Eliott"
        image="/_nuxt/assets/images/projects/mission-discovery.png"
        />

        <projectcard
        link="https://youtu.be/ozR_Qc24N2c" 
        description="Ce projet s’est déroulé au printemps 2023
        Nous avons collaboré avec la plateforme Pixabay qui avait besoin de mettre en avant les sons ajouter récemment.  Ce projet a été réaliser avec différents outils comme notre camera 360."
        image="/_nuxt/assets/images/projects/la-goutte.png"
        />
    </div>
</template>

<script setup>

import '~/assets/css/portfolio.css'


</script>