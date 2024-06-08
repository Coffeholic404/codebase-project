<script setup>
import { Icon } from "@iconify/vue";

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
</script>

<template>
    <div class="w-full fixed flex items-center justify-center z-[1001] pt-6">
        <div class="navbar w-full max-w-[64em] px-5 mx-auto h-[60px]">
            <div class="navlogo max-w-full w-[100px]">
                <img src="/assets/imgs/logo_white.svg" alt="">
            </div>
            <ul class="navlist text-sm font-medium text-titles-links cursor-pointer">
                <li>
                    <p popovertarget="support_modal">Support</p>
                </li>
                <li class=" relative">
                    <p class=" relative">Product</p>
                </li>
                <li>
                    <p>Company</p>
                </li>
                <li>
                    <p>Account</p>
                </li>
            </ul>
            <div class="navbtn">
                <button class="navbtn__logo text-xs text-white bg-primary py-[9px] px-[15px] rounded-2xl">Buy
                    template</button>
                <Icon icon="tabler:menu" class="menu" />
            </div>
        </div>

        <div popover id="support_modal">
            <div class="modal">
                <div class="modal-content">
                    <div class="modal-header">
                        <h2>Support</h2>
                        <span class="close">&times;</span>
                    </div>
                    <div class="modal-body">
                        <p>Some text in the Modal Body</p>
                        <p>Some other text...</p>
                    </div>
                </div>
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

@media (max-width: 479px) {
    .navbar.scrolled{
        margin-inline: 1em;
    }

    .navbar.scrolled {
        display: sticky;
        top: 0;
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
