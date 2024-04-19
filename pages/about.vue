<template>
    <navbar/>

    <div class="w100 p-relative toppart">
        <div class="title stroke p-absolute">
            A propos de nous
        </div>
        <h1 class="title">
            A propos de nous                
        </h1>
    </div>
    <section class="histoire">
        <h2>NOTRE HISTOIRE</h2>
        <p>
            Nous c’est Virtuowl, une agence de communication créée en 2020 durant la période de la pandémie de la COVID-19 qui permet de visiter autrement. Nous sommes situés à Nancy, dans le Grand-Est et nous proposons nos services jusqu’au Luxembourg.
        </p>
        <h2>NOS SERVICES</h2>
        <p>
            Nous proposons un service de réalité virtuelle afin de réaliser des visites immersives pour les entreprises souhaitant mettre en avant des lieux.              Notre solution est polyvalente. Que vous soyez une agence de tourisme, un musée, une agence immobilière ou tout autre type d’entreprise, notre service vous permet de présenter un lieu à votre clientèle à travers l’écran sans se déplacer. Grâce à nos visites virtuelles, vos clients peuvent explorer vos espaces sans avoir à se déplacer physiquement, ce qui ouvre de nouvelles opportunités pour augmenter votre visibilité et votre accessibilité.
            Notre approche garantit que nos services s'adaptent parfaitement à vos besoins spécifiques. En choisissant Virtuowl, vous optez pour une solution économique qui dynamise votre présence en ligne et vous permet de toucher un public plus large, où qu'il se trouve.
        </p>
    </section>

    <section class="valeurs">
        <h2>
            NOS VALEURS
        </h2>
        <div class="listVal">
            <div class="valItem">
            <img src="~/assets/images/fun-icon.svg" alt="cool emoji">
            <p>fun</p>
        </div>
        <div class="valItem">
            <img src="~/assets/images/group-icon.svg" alt="groupe">
            <p>Engagement Client </p>
        </div>
        <div class="valItem">
            <img src="~/assets/images/search-icon.svg" alt="loupe">
            <p>transparent</p>
        </div>

        </div>
    </section>

    <section class="equipe">
        <h2>L’équipe</h2>

        <div class="team">

            <teamcard 
            name="Jean" 
            description="Jean est un super dev qui gère de ouf il a plein de super compétences" 
            quote="Jadore la vie" 
            image="/_nuxt/assets/images/team/antoine.png"/>

            <teamcard 
            name="Jean" 
            description="Jean est un super dev qui gère de ouf il a plein de super compétences" 
            quote="Jadore la vie" 
            image="/_nuxt/assets/images/team/caro.png"/>

            <teamcard 
            name="Jean" 
            description="Jean est un super dev qui gère de ouf il a plein de super compétences" 
            quote="Jadore la vie" 
            image="/_nuxt/assets/images/team/lilou.png"/>

            <teamcard 
            name="Jean" 
            description="Jean est un super dev qui gère de ouf il a plein de super compétences" 
            quote="Jadore la vie" 
            image="/_nuxt/assets/images/team/lucas.png"/>

            <teamcard 
            name="Jean" 
            description="Jean est un super dev qui gère de ouf il a plein de super compétences" 
            quote="Jadore la vie" 
            image="/_nuxt/assets/images/team/milan.png"/>

            <teamcard 
            name="Jean" 
            description="Jean est un super dev qui gère de ouf il a plein de super compétences" 
            quote="Jadore la vie" 
            image="/_nuxt/assets/images/team/nicolas.png"/>

            <teamcard 
            name="Jean" 
            description="Jean est un super dev qui gère de ouf il a plein de super compétences" 
            quote="Jadore la vie" 
            image="/_nuxt/assets/images/team/nils.png"/>

            <teamcard 
            name="Jean" 
            description="Jean est un super dev qui gère de ouf il a plein de super compétences" 
            quote="Jadore la vie" 
            image="/_nuxt/assets/images/team/noemi.png"/>

            <teamcard 
            name="Jean" 
            description="Jean est un super dev qui gère de ouf il a plein de super compétences" 
            quote="Jadore la vie" 
            image="/_nuxt/assets/images/team/sarguis.png"/>

            <teamcard 
            name="Jean" 
            description="Jean est un super dev qui gère de ouf il a plein de super compétences" 
            quote="Jadore la vie" 
            image="/_nuxt/assets/images/team/valentin.png"/>

        </div>
    </section>

    <section class="idvisu">
        <h2>identité visuel</h2>
        <img src="/_nuxt/assets/images/charte_graphique.png" alt="charte graphique">
        <p>L’agence Virtu’Owl a choisi le hibou comme symbole complémentaire à son nom, en raison de sa capacité à voir tout autour de lui, similaire à l’objectif d’une caméra 360°.
 
Le logo de l’entreprise est une combinaison du nom et du pictogramme. 
La police utilisée est Poppins, une police sans empattement géométrique qui a gagné en popularité depuis son introduction. 
Elle prend en charge à la fois les systèmes d’écriture Devanagari et latin, ce qui en fait une addition internationale au genre, tout en restant simple et facile à lire. 

Les yeux du hibou sont mis en avant, car ils font référence à l’objectif de la caméra. 
Le logo lui-même se décline en différentes couleurs et arrière-plans. Les couleurs de la marque incluent un noir tiré vers un bleu nuit, ainsi qu’un bleu plus clair en référence à la technologie. Le blanc et le jaune sont utilisés pour mettre en valeur certains éléments, comme les yeux des hiboux, tandis qu’un bleu violet relie l’ensemble des couleurs et les met en valeur.</p>
    </section>


</template>

<style>


</style>
<script setup>

import '~/assets/css/about.css'

</script>