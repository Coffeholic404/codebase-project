<script setup>

</script>

<template>
    <div class="steps-section bg-neutral-800 curve-bottom">
        <div class="w-full z-[5] max-w-[72em] mx-auto px-[1.25em] relative">
            <div
                class="steps-bg-pattern-wrap w-full h-full flex justify-center items-center absolute top-0 bottom-0 right-0 left-0">
                <img src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d0749a8f715_bg-shape-003.png"
                    loading="lazy"
                    srcset="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d0749a8f715_bg-shape-003-p-500.png 500w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d0749a8f715_bg-shape-003-p-800.png 800w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d0749a8f715_bg-shape-003-p-1080.png 1080w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d0749a8f715_bg-shape-003-p-1600.png 1600w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d0749a8f715_bg-shape-003-p-2000.png 2000w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d0749a8f715_bg-shape-003-p-2600.png 2600w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d0749a8f715_bg-shape-003.png 3200w"
                    alt="" sizes="100vw"
                    class="steps-bg-pattern-image w-full object-contain mx-auto absolute top-auto bottom-auto left-0 right-0 max-w-full align-middle inline-block">
            </div>
            <div class="steps-margin mt-[8em]">
                <div class="content-centered w-full text-center flex flex-col items-center mx-auto relative">
                    <h2 class="steps-title-md max-w-[20ch]">What are the steps to launching a software site?</h2>
                </div>
            </div>
        </div>
    </div>
</template>



<style scoped>

.curve-bottom {
    width: auto;
    border-bottom-right-radius: 50%;
    border-bottom-left-radius: 50%;
    margin-inline: -40em;
    padding-bottom: 10em;
    padding-inline: 40em;
    position: relative;
    overflow: hidden;
}

.steps-section {
    padding-top: 5em;
}

.steps-title-md {
    color: var(--titles-links);
    letter-spacing: -.05em;
    font-size: 3.5em;
    font-weight: 700;
    line-height: 1;
}



@media (max-width: 479px) {
    .steps-margin {
        margin-bottom: 0;
        margin-left: 0;
        margin-right: 0;
        margin-top: 5em;
    }

    .steps-title-md {
        font-size: 2.5em;
    }
}

@media (min-width: 500px) and (max-width: 767px) {
    .steps-section {
        padding-top: 4em;
        padding-bottom: 4em;
    }

    .steps-margin {
        margin-bottom: 0;
        margin-left: 0;
        margin-right: 0;
        margin-top: 6em;
    }

    .steps-title-md {
        font-size: 3.125em;
    }

}

@media (min-width: 768px) and (max-width: 991px) {
    .steps-margin {
        margin-bottom: 0;
        margin-left: 0;
        margin-right: 0;
        margin-top: 7em;
    }

    .title-md {
        font-size: 3.5em;
    }
}
</style>