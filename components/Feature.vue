<script setup>
import { Icon } from "@iconify/vue";

  const { $gsap } = useNuxtApp();
  const card1 = ref(null);
  const card2 = ref(null);
  const card3 = ref(null);

  const one = ref(null);
  const two = ref(null);
  const three = ref(null);
  const four = ref(null);
  const five = ref(null);
  const six = ref(null);
  const seven = ref(null);
  const eight = ref(null);
  const nine = ref(null);
  const ten = ref(null);

  const img = ref(null);
  


onMounted(() => {
  const cards = [card1, card2, card3];
  cards.forEach((card, index) => {
    $gsap.fromTo(card.value, 
      { opacity: 0, y: 50 }, 
      { 
        opacity: 1, 
        y: 0,
        duration: 1,
        delay: index * 0.5, // Different delay for each card
        scrollTrigger: {
          trigger: card.value,
          start: 'top 80%', // Adjust based on when you want the animation to start
          end: 'bottom 50%',
          scrub: false,
          markers: false,
          toggleActions: 'restart none none none',
        },
      });
  });

  $gsap.fromTo(img.value, 
    { opacity: 0, x: 0}, 
    { 
      opacity: 1, 
      x: 992,
      delay:3,
      scrollTrigger: {
        trigger: img.value,
        start: 'top 80%', // Adjust based on when you want the animation to start
        end: 'top 50%',
        scrub: true,
        toggleActions: 'play none none none',
      },
    });
});
onMounted(() => {
  const cards = [one, two, three, four, five, six, seven, eight, nine, ten ];
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
});
</script>

<template>
    <div class="side-by-side mx-auto px-[1.25em]">
        <!-- left-side -->
        <div
        ref="img"
            class="animation2 right-side image-wrapper-3-4 rounded-xs fade-in-on-scroll w-full bg-accent pt-[124%] relative overflow-hidden rounded-[.5em] -left-[62rem]">
            <img src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d3e4ca8f66e_Rectangle-9.jpg"
                loading="lazy"
                srcset="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d3e4ca8f66e_Rectangle-9-p-500.jpeg 500w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d3e4ca8f66e_Rectangle-9-p-800.jpeg 800w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d3e4ca8f66e_Rectangle-9.jpg 1024w"
                alt="" sizes="(max-width: 479px) 92vw, (max-width: 767px) 71vw, (max-width: 991px) 72vw, 96vw"
                class="image-background"><img
                src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d25b0a8f6fe_blog-posts-06.png"
                loading="lazy"
                srcset="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d25b0a8f6fe_blog-posts-06-p-500.png 500w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d25b0a8f6fe_blog-posts-06.png 800w"
                alt="" sizes="(max-width: 479px) 92vw, (max-width: 767px) 71vw, (max-width: 991px) 72vw, 96vw"
                class="image-bg-contain">
        </div>


        <!-- <div class="side-by-side-img w-full rounded-[.5em] overflow-hidden relative">
            <img src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d3e4ca8f66e_Rectangle-9.jpg"
                loading="lazy"
                srcset="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d3e4ca8f66e_Rectangle-9-p-500.jpeg 500w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d3e4ca8f66e_Rectangle-9-p-800.jpeg 800w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d3e4ca8f66e_Rectangle-9.jpg 1024w"
                alt="" sizes="(max-width: 479px) 92vw, (max-width: 767px) 71vw, (max-width: 991px) 72vw, 96vw"
                class="image-background feature-img  w-full h-full filter-none object-cover max-w-full rounded-[.5em] align-middle inline-block">

            <img src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d25b0a8f6fe_blog-posts-06.png"
                loading="lazy"
                srcset="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d25b0a8f6fe_blog-posts-06-p-500.png 500w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d25b0a8f6fe_blog-posts-06.png 800w"
                alt="" sizes="(max-width: 479px) 92vw, (max-width: 767px) 71vw, (max-width: 991px) 72vw, 96vw"
                class="image-bg-contain feature-img   filter-none object-cover max-w-full rounded-[.5em] align-middle inline-block">
        </div> -->
        <!-- right side -->
        <div class=" rightside">
            <div class="feature margin-bottom margin-2xl mb-[2em]  max-w-[40em]">
                <div class="feature__wrapper max-width-xl w-full ">
                    <div class="margin-bottom margin-xl mb-[1.75em]">
                        <div ref="card1" class="feature-layout-grid caption-holder z-[5] w-full">
                            <div class="animation w-layout-grid feature-row-sm">
                                <div class="caption tracking-[.1em] uppercase text-[.625em] font-semibold">Feature ·
                                </div>
                                <div class="tracking-[.1em] uppercase text-[.625em] font-semibold opacity-[.5]">01</div>
                            </div>
                            <div class="line-holder">
                                <div class="line-animated"></div>
                            </div>
                        </div>
                    </div>
                    <div ref="card2"class="animation w-layout-grid feature-row-md">
                        <div
                            class="section-icon w-[2.75em] h-[2.75em] text-indigo-200 text-center rounded-full flex flex-col items-center justify-center">
                            <Icon icon="material-symbols:fingerprint" class=" text-indigo-200" />
                        </div>
                        <div class="section-text">
                            <div class="margin-bottom margin-base mb-[1em]">
                                <h2
                                    class="font-title text-titles-links tracking-[-.025em] relative text-[2.25em] font-bold leading-[1.2]">
                                    Works perfectly with your <span class="text-gradient__indigo">semantics</span>.</h2>
                            </div>
                            <div class="text-lg _48ch max-w-[48ch] tracking-[-.02] text-[1.25em] leading-[1.5]">Stand
                                out
                                online with a professional website, online store, or
                                portfolio. With Fouroom templates, you can turn any idea into a reality.</div>
                        </div>
                    </div>
                </div>
                <div class="animation w-layout-grid column-base mt-4">
                    <div ref="one" class="line-holder">
                        <div class="line-animated"></div>
                    </div>
                    <div ref="two" class="w-layout-grid feature-row fade-in-on-scroll">
                        <div class="text-sm">Add and edit schema
                            markup</div>
                        <div class="text-sm text-sm-icon">
                            <div class="material-icons-round">
                                <Icon icon="material-symbols:check" />
                            </div>
                        </div>
                    </div>
                    <div ref="three" class="line-holder">
                        <div class="line-animated"></div>
                    </div>
                    <div ref="four" class="w-layout-grid feature-row fade-in-on-scroll">
                        <div class="text-sm">Meta titles and meta
                            descriptions<br></div>
                        <div class="text-sm text-sm-icon">
                            <div>Unlimited</div>
                        </div>
                    </div>
                    <div ref="five" class="line-holder">
                        <div class="line-animated"></div>
                    </div>
                    <div ref="six" class="w-layout-grid feature-row fade-in-on-scroll">
                        <div class="text-sm">Indexing and sitemap
                            controls<br></div>
                        <div class="text-sm text-sm-icon">
                            <div>Easy edit</div>
                        </div>
                    </div>
                    <div ref="seven" class="line-holder">
                        <div class="line-animated"></div>
                    </div>
                    <div ref="eight" class="w-layout-grid feature-row fade-in-on-scroll">
                        <div class="text-sm">Robust 301 redirects
                            management<br></div>
                        <div class="text-sm text-sm-icon">
                            <div class="material-icons-round">
                                <Icon icon="material-symbols:check" />
                            </div>
                        </div>
                    </div>
                    <div ref="nine" class="line-holder">
                        <div class="line-animated"></div>
                    </div>
                    <div ref="ten" class="w-layout-grid feature-row fade-in-on-scroll">
                        <div class="text-sm">Simple image alt tag
                            editing<br></div>
                        <div class="text-sm text-sm-icon">
                            <div class="material-icons-round">
                                <Icon icon="material-symbols:check" />
                            </div>
                        </div>
                    </div>
                </div>
            </div>
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


/* @keyframes slide-fade-in {
    from {
        opacity: 0;
        transform: translateX(5vh);
    }
}

@media (prefers-reduced-motion: no-preference) {
    .animation {
        view-timeline-name: --item-timeline;
        animation: slide-fade-in both;
        animation-timeline: --item-timeline;
        animation-range: contain 0% contain 50%;
    }
} 
@keyframes slide-fade-in2 {
    from {
        opacity: 0;
        transform: translateY(5vh);
    }
}

@media (prefers-reduced-motion: no-preference) {
    .animation2 {
        view-timeline-name: --item-timeline;
        animation: slide-fade-in both;
        animation-timeline: --item-timeline;
        animation-range: contain 0% contain 50%;
    }
}  */
</style>