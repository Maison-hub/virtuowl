<template>
    <nav>

        <a @click="toggleMenu">Menu</a>
    </nav>
    <div class="burger-menu" :class="{ 'open': isOpen }">
        <div class="burger-icon" @click="toggleMenu">
            <div class="bar"></div>
            <div class="bar"></div>
        </div>
        <ul class="menu-items" v-if="isOpen">
           <NuxtLink to="/"><a>Home</a></NuxtLink>
            <NuxtLink to="/about"><a>à propos</a></NuxtLink>
            <NuxtLink to="/portfolio"><a>Portfolio</a></NuxtLink>
        </ul>
    </div>
</template>

<script>
    import { ref } from 'vue';

    export default {
        setup() {
            const isOpen = ref(false);

            const toggleMenu = () => {
                isOpen.value = !isOpen.value;
            };

            return {
                isOpen,
                toggleMenu
            };
        }
    }
</script>

<style>
nav{
    display: flex;
    align-items: center;
    justify-content: flex-end;
    width: 100%;
    padding: 18px 42px;
    position: sticky;
    top: 0px;
    z-index: 1000;
    background-color: #0b132b01;
    backdrop-filter: blur(10px);
}

nav a{
    cursor: pointer;
    font-size: 22px;
    font-weight: 700;
}

/* burger here */

.burger-menu {
    position: fixed;
    display: flex;
    justify-content: center;
    width: 0vw;
    top: 0;
    right: 0px;
    z-index: 1001;
    height: 100vh;
    background-color: var(--secondary-blue);
    transition: all .2s ease-in-out;
}

.burger-menu.open {
    width: 50vw;
}

.burger-icon {
    position: absolute;
    top: 20px;
    left: 20px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    width: 40px;
    height: 22px;
    cursor: pointer;
}

.burger-icon:hover .bar {
    background-color: var(--white);
}

.bar {
    width: 100%;
    height: 5px;
    border-radius: 10px;
    background-color: #000;
    transition: all 0.3s ease-in-out;
}

.open .bar:nth-child(1) {
    transform: translateY(8px) rotate(45deg);
}

.open .bar:nth-child(2) {
    transform: translateY(-8px) rotate(-45deg);
}

.menu-items {
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    padding: 30% 10px;
    list-style: none;
    opacity: 0;
    visibility: hidden;
    transition: opacity 0.3s ease-in-out, visibility 0s linear 0.3s;
}

.open .menu-items {
    opacity: 1;
    visibility: visible;
    transition-delay: 0s;
}

.menu-items a {
    text-decoration: underline;
    color: var(--blue);
    font-size: 5vw;
    font-weight: 900;
    cursor: pointer;
    transition: color 0.2s ease-in-out;
    text-transform: capitalize;
}

.menu-items a:hover {
    color: var(--white);
}

</style>