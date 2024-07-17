<script setup>
import { Icon } from "@iconify/vue";
const { $gsap } = useNuxtApp();
const feat = ref(null);
const feat2 = ref(null);
const img = ref(null);

const one = ref(null);
  const two = ref(null);
  const three = ref(null);
  const four = ref(null);
  const five = ref(null);

onMounted(() => {
    $gsap.fromTo(feat.value, 
    { opacity: 0, x: 0}, 
    { 
      opacity: 1, 
      x: 992,
      delay:1,
      ease: 'power2.inOut',
      scrollTrigger: {
        trigger: feat.value,
        start: 'top 80%', // Adjust based on when you want the animation to start
        end: 'top 50%',
        scrub: false,
        toggleActions: 'restart none none none',
      },
    });

    $gsap.fromTo(feat2.value, 
    { opacity: 0, x: 0}, 
    { 
      opacity: 1, 
      x: 992,
      delay:1,
      duration: 1,
      ease: 'power2.inOut',
      scrollTrigger: {
        trigger: feat2.value,
        start: 'top 80%', // Adjust based on when you want the animation to start
        end: 'top 50%',
        scrub: false,
        toggleActions: 'restart none none none',
      },
    });

    $gsap.fromTo(img.value, 
    { opacity: 0, y: 50 }, 
    { 
      opacity: 1, 
      y: 0,
      delay:2,
      ease: 'power3.inOut',
      scrollTrigger: {
        trigger: img.value,
        start: 'top 90%', // Adjust based on when you want the animation to start
        end: 'top 50%',
        scrub: false,
        toggleActions: 'restart none none none',
      },
    });


    const cards = [one, two, three, four, five];
  cards.forEach((card, index) => {
    $gsap.fromTo(card.value, 
      { opacity: 0, y: 50 }, 
      { 
        opacity: 1, 
        y: 0,
        duration: 1,
        delay: index * 0.2, // Different delay for each card
        scrollTrigger: {
          trigger: card.value,
          start: 'top 80%', // Adjust based on when you want the animation to start
          end: 'bottom 50%',
          scrub: false,
          markers: false,
          toggleActions: 'play none none none',
        },
      });
  });
})
</script>

<template>
    <div class="w-layout-grid side-by-side">
        <div class="feature-2 col-span-1 row-span-1">
            <div class="margin-bottom margin-2xl mb-[2em]">
                <div class="max-width-xl w-full max-w-[40em] ">
                    <div class="margin-bottom margin-xl mb-[1.75em]">
                        <div ref="feat" class="w-layout-grid caption-holder feature-layout-grid -left-[62rem]">
                            <div  class="w-layout-grid feature-row-sm ">
                                <div class="caption">Feature ·</div>
                                <div class="caption opacity-[.5]">02</div>
                            </div>
                            <div class="line-holder">
                                <div class="line-animated"></div>
                            </div>
                        </div>
                    </div>
                    <div ref="feat2" class="w-layout-grid feature-row-md -left-[62rem]">
                        <div class="section-icon-feature2 pink">
                            <Icon icon="material-symbols:fingerprint" />
                        </div>
                        <div class=" col-span-1 row-span-1">
                            <div class="margin-bottom margin-base mb-[1em]">
                                <h2
                                    class="font-title text-titles-links tracking-[-.025] relative text-[2.25em] font-bold leading-[1.2]">
                                    All the power you need, without <span class="text-gradient__pink ">plugins</span>.
                                </h2>
                            </div>
                            <div class="text-lg _48ch max-w-[48ch] tracking-[-.02em] text-1.25em leading-[1.5]">Webflow
                                gives you fine level control over SEO markup,
                                indexing rules, redirects, and more — push any changes live without relying on
                                engineers.</div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="w-layout-grid column-base ">
                <div ref="one" class="w-layout-grid column-sm fade-in-on-scroll">
                    <div class="w-layout-grid feature-row-sm  items-center">
                        <div class="square-h4  rounded-[.75em] overflow-hidden size-[1.8em] bg-pink-100 flex flex-col justify-center items-center text-center">
                            <div class="material-icons-outlined">
                                <div class="text-color-pink-500 text-pink-600">
                                    <Icon icon="material-symbols:inventory" /></div>
                            </div>
                        </div>
                        <h6 class="font-title text-titles-links tracking-[-.025em] relative my-0 text-[1em] font-semibold leading-[1.2]">Add and edit schema markup<br></h6>
                    </div>
                    <div id="w-node-e0cda5a5-075d-075a-3efd-657b1d91dd49-968e5ac7" class="text-sm">Add schema markup
                        so your content can be easily understood and represented in search engines.</div>
                </div>
                <div ref="two"  class="line-holder">
                    <div  class="line-animated"
                        ></div>
                </div>
                <div ref="three" class="w-layout-grid column-sm fade-in-on-scroll">
                    <div class="w-layout-grid feature-row-sm items-center">
                        <div class="square-h4 size-[1.8em] flex flex-col justify-center items-center overflow-hidden rounded-[.75em] bg-pink-100">
                            <div class="material-icons-outlined">
                                <div class="text-color-pink-500 text-pink-500">
                                    <Icon icon="material-symbols:upcoming-outline" /></div>
                            </div>
                        </div>
                        <h6 class="font-title text-titles-links tracking-[-.025em] relative my-0 text-[1em] font-semibold leading-[1.2]">Meta titles and meta descriptions<br></h6>
                    </div>
                    <div class="text-sm">Automatically
                        define meta titles and descriptions using fields in your CMS Collections.</div>
                </div>
                <div ref="four"  class="line-holder">
                    <div class="line-animated"
                        ></div>
                </div>
                <div ref="five" class="w-layout-grid column-sm fade-in-on-scroll"
                    >
                    <div class="w-layout-grid feature-row-sm items-center">
                        <div class="square-h4 size-[1.8em] flex flex-col justify-center items-center overflow-hidden rounded-[.75em] bg-pink-100">
                            <div class="material-icons-outlined">
                                <div class="text-color-pink-500 text-pink-500">
                                    <Icon icon="material-symbols-light:notifications-active-outline" />
                                </div>
                            </div>
                        </div>
                        <h6 class="font-title text-titles-links tracking-[-.025em] relative my-0 text-[1em] font-semibold leading-[1.2]">Indexing and sitemap controls<br></h6>
                    </div>
                    <div  class="text-sm">Easily edit and
                        update page titles and descriptions and publish changes in a click.</div>
                </div>
            </div>
        </div>
        <div
            ref="img"
            class="feature2-img image-wrapper-3-4 rounded-[.5em] fade-in-on-scroll bg-accent pt-[124%] relative overflow-hidden">
            <img src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d107ea8f688_Rectangle-8.jpg"
                loading="lazy"
                srcset="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d107ea8f688_Rectangle-8-p-500.jpeg 500w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d107ea8f688_Rectangle-8-p-800.jpeg 800w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d107ea8f688_Rectangle-8.jpg 1024w"
                alt="" sizes="(max-width: 479px) 92vw, (max-width: 767px) 71vw, (max-width: 991px) 72vw, 96vw"
                class="image-background"><img
                src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d5825a8f6f8_blog-posts-05.png"
                loading="lazy"
                srcset="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d5825a8f6f8_blog-posts-05-p-500.png 500w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d5825a8f6f8_blog-posts-05-p-800.png 800w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d5825a8f6f8_blog-posts-05-p-1080.png 1080w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d5825a8f6f8_blog-posts-05.png 1280w"
                alt="" sizes="(max-width: 479px) 92vw, (max-width: 767px) 71vw, (max-width: 991px) 72vw, 96vw"
                class="image-bg-contain">
        </div>
    </div>
</template>



<style scoped>
.side-by-side {
    width: 100%;
    display: grid;
    grid-column-gap: 5em;
    grid-row-gap: 5em;
    grid-template-rows: auto;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    position: relative;
}

.image-wrapper-3-4 {
    grid-area: span 1 / span 1 / span 1 / span 1;
}

.image-background {
    z-index: 0;
    width: 100%;
    height: 100%;
    filter: none;
    object-fit: cover;
    position: absolute;
    top: 0%;
    bottom: 0%;
    left: 0%;
    right: 0%;
}

.image-bg-contain {
    z-index: 0;
    width: 100%;
    height: 100%;
    object-fit: contain;
    position: absolute;
    top: 0%;
    bottom: 0%;
    left: 0%;
    right: 0%;
}

img {
    max-width: 100%;
    vertical-align: middle;
    display: inline-block;
}

.side-by-side .side-by-side-img {
    display: grid;
    grid-template-columns: 1fr;
    justify-content: center;
    align-items: center;
}

.side-by-side .side-by-side-img .feature-img {
    grid-column: 1/2;
    grid-row: 1/2;
}

.feature-layout-grid {
    display: grid;
    z-index: 5;
    width: 100%;
    grid-column-gap: 1em;
    grid-row-gap: 1em;
    grid-template-rows: auto;
    grid-template-columns: auto 1fr;
    align-items: center;
    grid-auto-columns: 1fr;
    position: relative;
}

.feature-row-sm {
    grid-column-gap: .5em;
    grid-row-gap: .5em;
    grid-template-rows: auto;
    grid-template-columns: auto;
    grid-auto-columns: auto;
    grid-auto-flow: column;
    justify-content: start;
    display: grid;
}



.line-holder {
    grid-area: span 1 / span 1 / span 1 / span 1;
    width: 100%;
    position: relative;
}

.line-animated {
    width: 100%;
    height: 1px;
    background-image: linear-gradient(to right, var(--border), rgba(33, 38, 45, 0));
    position: absolute;
    top: 0%;
    bottom: auto;
    left: 0%;
    right: 0%;
}

.feature-row-md {
    z-index: 5;
    grid-column-gap: 1.5em;
    grid-row-gap: 1.5em;
    grid-template-rows: auto;
    grid-template-columns: auto;
    grid-auto-columns: auto;
    grid-auto-flow: column;
    justify-content: start;
    display: grid;
    position: relative;
}

.section-icon {
    border: 3px solid var(--indigo-400);
    background-color: var(--indigo-700);
    background-image: radial-gradient(circle farthest-side at -50% 50%, var(--indigo-600), var(--indigo-700));
    box-shadow: inset 0 0 5px 0 var(--indigo-800), 0 8px 24px -8px var(--indigo-400);
    color: var(--indigo-200);
    font-size: 1.25em;
}

.section-text {
    grid-area: span 1 / span 1 / span 1 / span 1;
}

.text-gradient__indigo {
    background-image: linear-gradient(351deg, var(--sky-400) 23%, var(--indigo-600) 87%);
    -webkit-text-fill-color: transparent;
    -webkit-background-clip: text;
    background-clip: text;
    padding-right: .05em;
}

.column-base {
    z-index: 5;
    grid-column-gap: 1em;
    grid-row-gap: 1em;
    grid-template-rows: auto;
    grid-template-columns: 1fr;
    grid-auto-columns: 1fr;
    justify-items: start;
    display: grid;
    position: relative;
}

.feature-row {
    width: 100%;
    display: grid;
    grid-column-gap: .5em;
    grid-row-gap: .5em;
    grid-template-rows: auto;
    grid-template-columns: 1fr .5fr;
}

.rightside {
    grid-area: span 1 / span 1 / span 1 / span 1;
}

.text-sm {
    grid-area: span 1 / span 1 / span 1 / span 1;
    letter-spacing: -.005em;
    font-size: .875em;
    line-height: 1.25;
    position: relative;
}

.text-sm-icon {
    justify-self: end;
}

/* .feature-2 {
    grid-area: span 1 / span 1 / span 1 / span 1;
} */

.caption {
    letter-spacing: .1em;
    text-transform: uppercase;
    font-size: .625em;
    font-weight: 600;
}

.section-icon-feature2.pink {
    border-color: var(--pink-400);
    background-color: var(--pink-700);
    background-image: radial-gradient(circle farthest-side at -50% 50%, var(--pink-600), var(--pink-700));
    box-shadow: inset 0 0 5px 0 var(--pink-800), 0 8px 24px -8px var(--pink-400);
    color: var(--pink-200);
}

.section-icon-feature2 {
    width: 2.75em;
    height: 2.75em;
    border: 3px solid var(--indigo-400);
    background-color: var(--indigo-700);
    background-image: radial-gradient(circle farthest-side at -50% 50%, var(--indigo-600), var(--indigo-700));
    box-shadow: inset 0 0 5px 0 var(--indigo-800), 0 8px 24px -8px var(--indigo-400);
    color: var(--indigo-200);
    text-align: center;
    border-radius: 9999px;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-family: ICONS SHARP, sans-serif;
    font-size: 1.25em;
    display: flex;
}

.text-gradient__pink {
    background-image: linear-gradient(304deg, var(--red-400) 23%, var(--pink-600) 87%);
    -webkit-text-fill-color: transparent;
    -webkit-background-clip: text;
    background-clip: text;
    padding-right: .05em;
}

.column-sm {
    display: grid;
    grid-column-gap: .5em;
    grid-row-gap: .5em;
    grid-template-rows: auto;
    grid-template-columns: 1fr;
    grid-auto-columns: 1fr;
    justify-items: start;
    display: grid;
    position: relative;
}

.material-icons-outlined {
    text-transform: none;
    margin-top: -.05em;
    font-family: ICONS OUTLINED, sans-serif;
}
</style>import type { Feature } from "#build/components";
