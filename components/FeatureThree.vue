<script setup>
import { Icon } from "@iconify/vue";

const { $gsap } = useNuxtApp();
  const card1 = ref(null);
  const card2 = ref(null);

  const one = ref(null);
  const two = ref(null);
  const three = ref(null);
  const four = ref(null);
  const five = ref(null);
  const six = ref(null);

  onMounted(() => {
  const cards = [card1, card2];
  cards.forEach((card, index) => {
    $gsap.fromTo(card.value, 
      { opacity: 0, x: 0 }, 
      { 
        opacity: 1, 
        x: 992,
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
  
});

onMounted(() => {
  const cards = [one, two, three, four, five,six];
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
    <div class="feature3-container w-full max-w-[64em] mx-auto px-[1.25em] static">
        <div class="feature mb-[2.5em] margin-bottom margin-4xl">
            <div class="max-width-xl w-full max-w-[40em]">
                <div class="feature-heading mb-[1.75em] margin-bottom margin-xl">
                    <div ref="card1" class="caption-holder -left-[62rem]">
                        <div class="w-layout-grid feat-row-sm ">
                            <div class="heading-caption leading-[.1em] uppercase text-[.625em] font-semibold">Feature ·
                            </div>
                            <div class="leading-[.1em] uppercase text-[.625em] font-semibold opacity-[.5]">02</div>
                        </div>

                        <div c class="line-holder">
                            <div class="line-animated"></div>
                        </div>
                    </div>
                </div>


                <div ref="card2" class="w-layout-grid feat-row-md -left-[62rem]">
                    <div class="section-icon-amber">
                        <Icon icon="material-symbols:fingerprint" class=" text-indigo-200" />
                    </div>
                    <div class=" section-content">
                        <div class="margin-bottom sec-margin-base mb-[1em]">
                            <h2 class="title-md">Website content <span class="text-amber">management</span>
                                made easy.</h2>
                        </div>
                        <div class="text-lg  max-w-[48ch]">Webflow gives you fine level control over SEO markup,
                            indexing rules,
                            redirects, and more — push any changes live without relying on engineers.</div>
                    </div>
                </div>
            </div>
        </div>

        <div class="tab-holder pl-[4em]">
            <div class="tab-menu" >

                <a 
                ref="one"
                href="" 
                class="tab-menu-click tab-menu-current  flex text-center rounded-[.375em] justify-center items-center py-[2em] text-[.875em] font-semibold leading-[1]">
                    <p>Kanban</p>
                </a>
                <a 
                ref="two"
                href="" class="tab-link-simple tab-menu-click flex text-center rounded-[.375em] justify-center items-center py-[2em] text-[.875em] font-semibold leading-[1]">
                    <p>User Story Map</p>
                </a>
                <a 
                ref="three"
                href="" class="tab-link-simple tab-menu-click flex text-center rounded-[.375em] justify-center items-center py-[2em] text-[.875em] font-semibold leading-[1]">
                    <p>Retrospective</p>
                </a>
                <a 
                ref="four"
                href="" class="tab-link-simple tab-menu-click flex text-center rounded-[.375em] justify-center items-center py-[2em] text-[.875em] font-semibold leading-[1]">
                    <p>PI Planning</p>
                </a>
                <a 
                ref="five"
                href="" class="tab-link-simple tab-menu-click flex text-center rounded-[.375em] justify-center items-center py-[2em] text-[.875em] font-semibold leading-[1]">
                    <p>Daily Standup</p>
                </a>
            </div> 

            <div ref="six" class="tab-simple-content static overflow-hidden ">
                    <div class=" static">
                        <img srcset="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d7779a8f704_blog-post-07-p-1080.jpeg 1080w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d7779a8f704_blog-post-07.jpg 1280w" alt="" src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d7779a8f704_blog-post-07.jpg" loading="lazy" sizes="(max-width: 479px) 92vw, (max-width: 767px) 95vw, (max-width: 991px) 96vw, 90vw" class="image-contain rounded-[.5em] relative overflow-hidden max-w-full align-middle inline-block z-[5] w-full leading-[1] object-contain">
                    </div>
            </div> 
        </div>
    </div>
</template>



<style scoped>


.caption-holder {
    display: grid;
    z-index: 5;
    width: 100%;
    grid-column-gap: 1em;
    grid-row-gap: 1em;
    grid-template-rows: auto;
    grid-template-columns: auto 1fr;
    align-items: center;
    position: relative;
}

.feat-row-sm {
    gap: .5em;
    grid-template-rows: auto;
    grid-template-columns: auto;
    grid-auto-columns: auto;
    grid-auto-flow: column;
    justify-content: start;
    display: grid;
}

.feat-row-md {
    z-index: 5;
    gap: 1.5em;
    grid-template-rows: auto;
    grid-template-columns: auto;
    grid-auto-columns: auto;
    grid-auto-flow: column;
    justify-content: start;
    display: grid;
    position: relative;
}

.section-icon-amber {
    border-color: var(--amber-500);
    background-color: var(--amber-700);
    background-image: radial-gradient(circle farthest-side at -50% 50%, var(--amber-600), var(--amber-700));
    box-shadow: inset 0 0 5px 0 var(--amber-800), 0 8px 24px -8px var(--amber-400);
    outline-color: var(--amber-400);
    color: var(--amber-200);
    text-align: center;
    border-radius: 9999px;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-family: ICONS SHARP, sans-serif;
    font-size: 1.25em;
    display: flex;
    width: 2.75em;
    height: 2.75em;
    border: 3px solid
}

.line-holder {
    width: 100%;
    position: relative;
    grid-area: span 1 / span 1 / span 1 / span 1;
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

.section-content{
    grid-area: span 1 / span 1 / span 1 / span 1;
}

.title-md {
    color: var(--titles-links);
    letter-spacing: -.05em;
    font-size: 3.5em;
    font-weight: 700;
    line-height: 1;
}

.text-amber{
    background-image: linear-gradient(191deg, var(--yellow-300) 25%, var(--amber-600) 87%);
    -webkit-text-fill-color: transparent;
    -webkit-background-clip: text;
    background-clip: text;
    padding-right: .05em;
}

.text-lg {
    letter-spacing: -.02em;
    font-size: 1.25em;
    line-height: 1.5;
}

.tab-menu-click {
    transition: opacity .25s;
    letter-spacing: -.01em;
}

.tab-menu-current {
    background-color: var(--background);
    opacity: 1;
    color: var(--amber-400);
    background-image: linear-gradient(rgba(245, 158, 11, .1), rgba(245, 158, 11, .1));
    box-shadow: inset 0 0 0 1px rgba(251, 191, 36, .4);
}

.tab-link-simple {
    background-color: var(--neutral-800);
    opacity: .5;
    color: var(--titles-links);
    text-align: center;
    letter-spacing: -.01em;
    border-radius: .375em;
    flex: 1;
    padding-top: 2em;
    padding-bottom: 2em;
    font-size: .875em;
    font-weight: 600;
    line-height: 1;
    transition: opacity .25s;
}

.tab-link-simple:hover {
    opacity: 1;
}

.tab-menu {
    z-index: 5;
    grid-column-gap: .5em;
    grid-row-gap: .5em;
    grid-template-rows: auto;
    grid-template-columns: 1fr;
    grid-auto-columns: 1fr;
    grid-auto-flow: column;
    margin-bottom: 1em;
    display: grid;
}


@media (max-width: 479px) {
    .feature {
        margin-top: 0;
        margin-left: 0;
        margin-right: 0;
        margin-bottom: 1.875em;
    }

    .feature-heading {
        margin-top: 0;
        margin-left: 0;
        margin-right: 0;
        margin-bottom: 1.375em;
    }

.section-content{
        grid-area: 2 / 1 / 3 / 2;
}

.sec-margin-base {
        margin-top: 0;
        margin-left: 0;
        margin-right: 0;
    }

    .title-md {
        font-size: 2.5em;
    }

    .text-lg {
        font-size: 1.125em;
    }

    .tab-holder {
        padding-left: 0;
    }

}

@media (min-width: 500px) and (max-width: 767px){
    .feature {
        margin-top: 0;
        margin-left: 0;
        margin-right: 0;
        margin-bottom: 2.125em;
    }

    .feature-heading {
        margin-top: 0;
        margin-left: 0;
        margin-right: 0;
        margin-bottom: 1.5em;
    }

    .feat-row-md{
        gap: 1em .5em;
    }

    .sec-margin-base {
        margin-top: 0;
        margin-left: 0;
        margin-right: 0;
        margin-bottom: .875em;
    }

    .title-md {
        font-size: 3.125em;
    }

    .text-lg {
        font-size: 1.125em;
    }


}

@media (min-width: 768px) and (max-width: 991px) {
    .feature {
        margin-top: 0;
        margin-left: 0;
        margin-right: 0;
        margin-bottom: 2.5em;
    }

    .feature-heading {
        margin-top: 0;
        margin-left: 0;
        margin-right: 0;
        margin-bottom: 1.625em;
    }

    .title-md {
        font-size: 3.5em;
    }

    .tab-simple-menu {
        width: 100%;
        display: flex;
        overflow: scroll;
    }

}
</style>