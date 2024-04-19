<template>
    <div class="burger-menu" :class="{ 'open': isOpen }">
        <div class="burger-icon" @click="toggleMenu">
            <div class="bar"></div>
            <div class="bar"></div>
            <div class="bar"></div>
        </div>
        <ul class="menu-items" v-if="isOpen">
            <a>Home</a>
            <a>About</a>
            <a>Contact</a>
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
.burger-menu {
    position: fixed;
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
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    width: 30px;
    height: 20px;
    cursor: pointer;
}

.bar {
    width: 100%;
    height: 3px;
    background-color: #000;
    transition: transform 0.3s ease-in-out;
}

.open .bar:nth-child(1) {
    transform: translateY(8px) rotate(45deg);
}

.open .bar:nth-child(2) {
    opacity: 0;
}

.open .bar:nth-child(3) {
    transform: translateY(-8px) rotate(-45deg);
}

.menu-items {
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    top: 60px;
    padding: 10px;
    list-style: none;
    opacity: 0;
    visibility: hidden;
    transition: opacity 0.3s ease-in-out, visibility 0s linear 0.3s;
    background-color: red;
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
}
</style>