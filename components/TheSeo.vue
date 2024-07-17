<script setup>

</script>

<template>
    <div class="seo__wrapper text-center w-full">
        <div class=" ">
            <h4 class="seo__heading relative">01 .search engine optimization</h4>
        </div>
        <div class=" flex flex-col items-center justify-center mt-8">
            <h2 class=" title-lg max-w-[12ch] leading-[1] tracking-[-.05] text-[4em] font-bold text-titles-links ">
                SEO controls, under control
            </h2>
            <div class="title-sm max-w-[32em] mt-6">
                <p class=" tracking-[-.01] text-[1.5em] text-center  ">
                    Optimize your website SEO with fine-tuned controls, high-performance hosting, and flexible content management tools.
                </p>
            </div>
        </div>
        <div class="layout_cards">
            <div class="cards">
                <UICards />
            </div>
        </div>
    </div>
</template>

<style scoped>
.seo__wrapper {
    background-image: url(/assets/imgs/bg-shape-002-p-2000.png);
    background-size: 100% 100%;
    /* background-position: top 30% left 10%; */
    background-repeat: no-repeat;
    /* height: 100dvh; */
}
.seo__heading {
    letter-spacing: .1em;
    text-transform: uppercase;
    font-size: .625em;
    font-weight: 600;
}

.seo__heading::before {
    --text: #a7b5c3;
    content: "";
    position: absolute;
    top: 50%;
    left: 12%;
    /* transform: translateX(-50%); */
    width: 30%;
    height: 1px;
    background-image: linear-gradient(to right, var(--border), rgba(33, 38, 45, 0));
    transform: rotate(180deg);
}

.seo__heading::after {
    --text: #a7b5c3;
    content: "";
    position: absolute;
    top: 50%;
    right: 12%;
    /* transform: translateX(-50%); */
    width: 30%;
    height: 1px;
    background-image: linear-gradient(to right, var(--border), rgba(33, 38, 45, 0));
}

.title-sm {
    letter-spacing: -.01em;
    font-size: 1.5em;
}


@media (max-width: 479px) {

  .title-lg {
        letter-spacing: -.01em;
        font-size: 1.875em;
    }

    .title-sm {
        font-size: .75em;
    }
}

@media (min-width: 500px) and (max-width: 766px){
    .title-lg {
        font-size: 3.25em;
    }

    .title-sm {
        font-size: 1.175em;
        line-height: 1.4;
    }
}

@media (min-width: 768px) and (max-width: 991px) {
    .title-lg {
        font-size: 3.25em;
    }
}
</style>