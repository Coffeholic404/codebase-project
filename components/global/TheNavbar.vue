<script setup>
import { Icon } from "@iconify/vue";

const isNavbarOpen = ref(false);

// Function to handle scroll event
const handleScroll = () => {
    const navbar = document.querySelector('.navbar');
    if (navbar) {
        if (window.scrollY > 0) {
            navbar.classList.add('scrolled'); // Add a class when scrolled
        } else {
            navbar.classList.remove('scrolled'); // Remove the class when not scrolled
        }
    }
};

// Listen for scroll events
onMounted(() => {
    window.addEventListener('scroll', handleScroll);
});

// Clean up event listener when component is unmounted
onUnmounted(() => {
    window.removeEventListener('scroll', handleScroll);
});

const toggleNavbar = () => {
    isNavbarOpen.value = !isNavbarOpen.value;
};
</script>

<template>
    <div :class="{'navbarmobile': isNavbarOpen, 'w-full': true, 'fixed': true, 'flex': true, 'items-center': true, 'justify-center': true, 'z-[1001]': true, 'pt-6': true}">
        <div class="navbar  w-full max-w-[64em] px-5 mx-auto h-[60px]">
            <div class="navlogo max-w-full w-[100px]">
                <img src="/assets/imgs/logo_white.svg" alt="">
            </div>
            <ul class="navlist text-sm font-medium text-titles-links cursor-pointer">
                <li>
                    <p>Support</p>
                </li>
                <li class="pad-top">
                    <p >Product</p>
                </li>
                <li class="pad-top">
                    <p>Company</p>
                </li>
                <li class="pad-top">
                    <p>Account</p>
                </li>
            </ul>
            <div class="navbtn">
                <button class="navbtn__logo text-xs text-white bg-primary py-[9px] px-[15px] rounded-2xl">Buy
                    template</button>
                <Icon icon="tabler:menu" class="menu"  v-show="!isNavbarOpen" @click="toggleNavbar"/>
                <Icon icon="material-symbols:close" v-show="isNavbarOpen" @click="toggleNavbar"/>
            </div>
        </div>

    </div>
</template>

<style scoped>
.navbar {
    display: grid;
    grid-template-columns: auto 1fr auto;
    grid-template-rows: auto;
    justify-content: center;
    align-items: center;
    gap: 24px;
    transition: background-color 0.3s ease; /* Add smooth transition */
}

.BgColour {
    background-color: var(--primary);
}

.navlogo {
    grid-column: 1/2;
}

.navlist {
    grid-column: 2/3;
    justify-self: start;
    display: flex;
    gap: 24px;
    align-items: center;
}

.navbtn {
    grid-column: 3/4;
}

.navbarmobile {
    min-width: 200px;
    /* position: absolute;
    top: 100%;
    left: 0;
    right: 0; */
    overflow: visible;
    display: block !important;
    background-color: var(--neutral-700);
    height: 64%;
    padding-top: 6em;
}

@media (max-width: 479px) {
    .navbar.scrolled{
        margin-inline: 1em;
    }

    .navbar.scrolled {
        display: sticky;
        top: 0;
    }

    /* .navbar-mobile .navlist {
        display: block !important;
    } */

    .navbarmobile .navbar {
        display: grid;
        grid-template-columns: 1fr .8fr;
        grid-template-rows: auto;
        gap: 2em;
        justify-content: center;
        height: 60%;
        margin: 0;
    }

    .navbarmobile .navlogo {
        grid-column: 1/2;
        grid-row: 1/2;
    }

    .navbarmobile .navlist {
        grid-column: 1/2;
        grid-row: 2/3;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        gap: 2em;
        padding-top: .5em;
        padding-inline: 1em ;
        /* font-size: 14px;
        font-weight: 500; */
    }
    .navbarmobile .navlist li p {
        font-size: 14px;
        font-weight: 500;
        /* letter-spacing: .03em; */
    }
    .navbarmobile .navlist .pad-top{
        margin-top: 2em;
    }
}

@media (min-width: 991px) {
    .menu {
        display: none;
    }
}

@media (min-width: 768px) and (max-width: 991px) {
    .navlist {
        display: none;
    }

    .navbar {
        grid-template-columns: auto 1fr;
    }

    .navlogo {
        grid-column: 1/2;
    }

    .navbtn {
        grid-column: 2/3;
        justify-self: end;
        display: flex;
        gap: 24px;
        justify-content: center;
        align-items: center;
    }
}

@media (max-width: 767px) {
    .navbtn__logo {
        display: none;
    }

    .navlist {
        display: none;
    }

    .navbar {
        grid-template-columns: auto 1fr;
    }

    .navlogo {
        grid-column: 1/2;
    }

    .navbtn {
        grid-column: 2/3;
        justify-self: end;
        display: flex;
        gap: 24px;
        justify-content: center;
        align-items: center;
    }
}

.navbar.scrolled {
    background-color: var(--primary);
    border-radius: 1rem;
}
.navbar.scrolled .navbtn__logo{
    background-color: var(--blue-500);
}
</style>
