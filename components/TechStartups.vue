<script setup>

</script>

<template>
    <div class="logo-tile-section">
        <div class="logo-tile-caption h-[2em] text-center rounded-full flex justify-center items-center px-[1em]">Join&nbsp;over&nbsp;2,000&nbsp;tech&nbsp;startups</div>
        <div class="logo-tile-list ">
            <div class="logo-tile"><img
                    src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d4615a8f6c1_logo-05-black.svg"
                    loading="lazy" alt="" class="client-logo-base"></div>
            <div class="logo-tile"><img
                    src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949dd4cda8f6bb_logo-07-black.svg"
                    loading="lazy" alt="" class="client-logo-base"></div>
            <div class="logo-tile"><img
                    src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d7aaea8f6bc_logo-01-black.svg"
                    loading="lazy" alt="" class="client-logo-base"></div>
            <div class="logo-tile"><img
                    src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d6870a8f6b9_logo-06-black.svg"
                    loading="lazy" alt="" class="client-logo-base"></div>
            <div class="logo-tile"><img
                    src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949dc518a8f6b6_logo-02-black.svg"
                    loading="lazy" alt="" class="client-logo-base"></div>
            <div class="logo-tile"><img
                    src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d40bfa8f6b3_logo-04-black.svg"
                    loading="lazy" alt="" class="client-logo-base"></div>
        </div>
    </div>
</template>


<style scoped>
    .logo-tile-section {
    flex-direction: column;
    align-items: center;
    margin-top: 2em;
    display: flex;
    position: relative;
}

    .logo-tile-caption {
    background-color: var(--background);
    text-transform: none;
    font-size: .75em;
    font-weight: 500;
    position: absolute;
    top: -1em;
    box-shadow: inset 0 0 0 1px var(--neutral-600), 0 8px 24px -8px var(--neutral-400);
}

.logo-tile-list {
    width: 100%;
    display: grid;
    gap: 1px;
    grid-template-rows: auto;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;
    margin-bottom: 1px;
}

.logo-tile {
    height: 12em;
    background-color: var(--neutral-800);
    justify-content: center;
    align-items: center;
    display: flex;
    background-color: var(--neutral-800);
}

.client-logo-base {
    height: 2em;
    max-width: 6em;
}


@media (max-width: 479px) {
    .logo-tile-list {
        grid-template-columns: 1fr 1fr;
    }

}

@media (min-width: 500px) and (max-width: 767px){
   

}

@media (min-width: 768px) and (max-width: 991px) {
    .logo-tile-list {
        grid-template-columns: 1fr 1fr 1fr;
    }
}
</style>