<script setup>
import { Icon } from "@iconify/vue";

const { $gsap } = useNuxtApp();
const image = ref(null);

onMounted(()=> {
  $gsap.fromTo(image.value, 
    { opacity: 0, x: 0}, 
    { 
      opacity: 1, 
      x: -1232,
      duration: 1,

      easy: 'power3.inOut',
      scrollTrigger: {
        trigger: image.value,
        start: 'top 80%', // Adjust based on when you want the animation to start
        end: 'top 50%',
        scrub: false,
        toggleActions: 'play none none none',
      },
    });
});
</script>

<template>
    <div class="bg-neutral-800 curve-bottom">
        <div class="section padding-bottom w-full pb-[5em] relative">
            <div class="container-md z-[5]w-full max-w-[56em] mx-auto px-[1.25em] relative">
                <div ref="image" class="feature-3-column relative -right-[77rem]">
                    <div class="column-base relative">
                        <div class="square-h3 bg-neutral-700">
                            <div class="material-icons-outlined">
                                <div class="text-white"><Icon icon="material-symbols:inventory" /></div>
                            </div>
                        </div>
                        <div class="content col-span-1 row-span-1 ">
                            <h6 class="font-title text-titles-links">Flexible CMS</h6>
                            <div class="text-sm ">Create whatever content types your site needs with a flexible, visual
                                CMS.</div>
                        </div>
                        <div class="_3x-feature-line-bottom">
                        </div>
                    </div>
                    <div class="column-base relative">
                        <div class="square-h3 bg-neutral-700">
                            <div class="material-icons-outlined">
                                <div class="text-white">
                                    <Icon icon="material-symbols-light:notifications-active-outline" />
                                </div>
                            </div>
                        </div>
                        <div class="content col-span-1 row-span-1 ">
                            <h6 class="font-title ">Simple editing tools</h6>
                            <div class="text-sm">Empower content teams to easily, independently produce at scale with
                                the Editor.</div>
                        </div>
                        <div class="_3x-feature-line-bottom">
                        </div>
                        <div  class="_3x-feature-line-left">
                        </div>
                    </div>

                    <div class="column-base relative">
                        <div class="square-h3 bg-neutral-700">
                            <div class="material-icons-outlined">
                                <div class="text-white">
                                    <Icon icon="material-symbols-light:notifications-active-outline" />
                                </div>
                            </div>
                        </div>
                        <div class="content col-span-1 row-span-1 ">
                            <h6 class="font-title">Speed, scale, and security</h6>
                            <div class="text-sm">Publish to a world-class hosting stack that can handle any traffic you
                                throw at it.<br></div>
                        </div>
                        <div class="_3x-feature-line-bottom">
                        </div>
                        <div
                            class="_3x-feature-line-left hide-mobile"></div>
                    </div>

                    <div class="column-base relative">
                        <div class="square-h3 bg-neutral-700">
                            <div class="material-icons-outlined">
                                <div class="text-white">
                                    <Icon icon="material-symbols:inventory" />
                                </div>
                            </div>
                        </div>
                        <div class="content col-span-1 row-span-1 ">
                            <h6 class="font-title">Easy edits and publishing</h6>
                            <div class="text-sm">Let clients and colleagues update content with an intuitive Editor.<br>
                            </div>
                        </div>
                        <div 
                            class="_3x-feature-line-bottom tablet hide"></div>
                        <div 
                            class="_3x-feature-line-left tablet"></div>
                    </div>

                    <div class="column-base relative">
                        <div class="square-h3 bg-neutral-700">
                            <div class="material-icons-outlined">
                                <div class="text-white">
                                    <Icon icon="material-symbols:upcoming" />
                                </div>
                            </div>
                        </div>
                        <div class="content col-span-1 row-span-1 " >
                            <h6 class="font-title">A complete platform</h6>
                            <div class="text-sm">Integrate marketing tools, collect form data, store backups, and
                                more.<br><br></div>
                        </div>
                        <div
                            class="_3x-feature-line-left hide-mobile"></div>
                        <div 
                            class="_3x-feature-line-bottom mobile"></div>
                    </div>

                    <div class="column-base relative">
                        <div class="square-h3 bg-neutral-700">
                            <div class="material-icons-outlined">
                                <div class="text-white">
                                    <Icon icon="material-symbols:hub" />
                                </div>
                            </div>
                        </div>
                        <div class="content col-span-1 row-span-1 ">
                            <h6 class="font-title">Export code for download</h6>
                            <div class="text-sm">Download a ZIP of all your HTML, CSS, JavaScript, images.<br></div>
                        </div>
                        <div class="_3x-feature-line-left">
                        </div>
                    </div>
                </div>
            </div>
            <div class="bg-pattern-wrap"><img
                    src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d359ba8f716_bg-shape-004.png"
                    loading="lazy"
                    srcset="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d359ba8f716_bg-shape-004-p-500.png 500w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d359ba8f716_bg-shape-004-p-800.png 800w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d359ba8f716_bg-shape-004-p-1080.png 1080w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d359ba8f716_bg-shape-004-p-1600.png 1600w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d359ba8f716_bg-shape-004-p-2000.png 2000w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d359ba8f716_bg-shape-004-p-2600.png 2600w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d359ba8f716_bg-shape-004.png 3200w"
                    alt="" sizes="10vw" class="bg-pattern-image"></div>
        </div>
    </div>
</template>



<style scoped>
.curve-bottom {
    width: auto;
    border-bottom-right-radius: 50%;
    border-bottom-left-radius: 50%;
    margin-left: -40em;
    margin-right: -40em;
    padding-bottom: 10em;
    padding-left: 40em;
    padding-right: 40em;
    position: relative;
    overflow: hidden;
}

.feature-3-column {
    display: grid;
    width: 100%;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: auto;
    gap: 4em;
}

.column-base {
    display: grid;
    z-index: 5;
    grid-template-columns: 1fr;
    grid-template-rows: auto;
    gap: 1em;
    justify-items: start;
}

.square-h3 {
    width: 2.25em;
    height: 2.25em;
    text-align: center;
    display: flex;
    justify-content:center;
    align-items: center;
    position: relative;
    border-radius: .5em;
    overflow: hidden;
}

.font-title {
    letter-spacing: -.025em;
    position: relative;
    color: var(--titles-links);
}

h6 {
    letter-spacing: 0;
    margin-top: 0;
    margin-bottom: 0;
    font-size: 1em;
    font-weight: 600;
    line-height: 1.2;
}

.text-sm {
    letter-spacing: -.005em;
    font-size: .875em;
    line-height: 1.25;
    position: relative;
}

._3x-feature-line-bottom {
    grid-area: span 1 / span 1 / span 1 / span 1;
    height: 1px;
    background-color: var(--neutral-600);
    position: absolute;
    top: auto;
    bottom: -1.5em;
    left: 0%;
    right: 0%;
}

._3x-feature-line-left {
    grid-area: span 1 / span 1 / span 1 / span 1;
    width: 1px;
    background-color: var(--neutral-600);
    position: absolute;
    top: 0%;
    bottom: 0%;
    left: -1.5em;
    right: auto;
}



._3x-feature-line-bottom.mobile,
._3x-feature-line-bottom.tablet,
._3x-feature-line-left.tablet{
        display: none;
    }

@media (max-width:479px) {
    ._3x-feature-line-left {
        display: none;
    }
    ._3x-feature-line-left, ._3x-feature-line-left.tablet {
        display: none;
    }

    ._3x-feature-line-bottom.mobile {
        display: block;
    }

    ._3x-feature-line-bottom.tablet {
        display: block;
    }

    .feature-3-column {
        width: 100%;
        grid-template-columns: 1fr;
    }
}

@media (max-width:767px) {
    .hide-mobile {
        display: none;
    }

    ._3x-feature-line-bottom.tablet .hide {
        display: none;
    }
}

@media (max-width:991px) {
    /* ._3x-feature-line-bottom.tablet {
        display: block;
    } */
    
    /* .feature-3-column{
        grid-template-columns: 1fr 1fr;
        grid-auto-flow: row;
    } */
}

@media (min-width:991px) {
    ._3x-feature-line-bottom .mobile {
        display: none;
    }


}
</style>