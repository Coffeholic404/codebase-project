<script setup>
import { Icon } from "@iconify/vue";

import { onMounted, ref } from 'vue';
  const { $gsap } = useNuxtApp();
  const card1 = ref(null);
  const card2 = ref(null);
  const card3 = ref(null);
  


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
});

</script>

<template>
<div ref="card1" class="animation card-1 card-wrapper mt-10">
            <div class="card-body bg-neutral-800 w-[330px] h-[360px] rounded-lg mx-auto p-5">
                <h4 class="card-body__heading text-titles-links tracking-[-.025em] text-[1.5em] font-bold leading-[1.2]">01.</h4>
                <div class=" bg-neutral-800 rounded-[.5em] overflow-hidden">
                    <div class=" w-[85%]  h-[96px]   rounded-md mx-auto my-[2.75em]">
                        <div class="snippet__body flex justify-center items-center min-h-[6em] rounded-[.375em] p-[.75em] bg-neutral-700">
                            <div class=" flex justify-center items-center relative">
                                <div class="dot-list relative">
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                    <div class="dot w-[2px] h-[2px] bg-accent opacity-[.15] rounded-[24%]"></div>
                                </div>
                                <div class="snippt-block  absolute">
                                    <div class="block-copy  min-h-[1.75em] ">
                                    </div>
                                    <div class="block-copy__icon rounded-full px-[.5em]  aspect-square flex justify-center items-center">
                                        <Icon icon="material-symbols:manage-search" class=" rounded-full"/>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-sm">
                    <h5 class=" text-titles-links tracking-[-.025em] font-bold text-[1.25em] leading-[1.2]">Speed</h5>
                    <div class=" opacity-[.6] font-semibold">
                        <p>
                            100+ datacenters worldwide means your site loads fast for every visitor.
                        </p>
                    </div>
                </div>
            </div>
        </div>

        <div ref="card2" class="animation card-2  card-wrapper mt-10">
            <div class="card-body bg-neutral-800 w-[330px] h-[360px] rounded-lg mx-auto p-5">
                <h4 class="card-body__heading text-titles-links tracking-[-.025em] text-[1.5em] font-bold leading-[1.2]">02.</h4>
                <div class=" bg-neutral-800 rounded-[.5em] overflow-hidden">
                    <div class=" w-[85%]  h-[96px]   rounded-md mx-auto my-[2.75em]">
                        <div class="snippet__body flex flex-col justify-start items-stretch min-h-[6em] rounded-[.375em] p-[.75em] bg-neutral-700 ">
                            <div class=" w-full avatar-wrap">
                                <div class="first w-full h-[5px] bg-neutral-600 rounded-full avatar-wrap-first"></div>
                                <div class="sec w-full h-[5px] bg-neutral-600 rounded-full"></div>
                                <div class="thi w-full h-[5px] bg-neutral-600 rounded-full"></div>
                                <div class="forth flex items-center avatar-wrap-sec">
                                    <img src="/assets//imgs/avatar-closeup-woman-03-p-500.jpeg" alt="" class=" w-[2em] h-[2em] object-cover rounded-full max-w-full align-middle inline-block">
                                    <img src="/assets/imgs/avatar-closeup-woman-02.jpg" alt="" class=" w-[2em] h-[2em] object-cover rounded-full max-w-full align-middle inline-block snippit-avtar">
                                    <img src="/assets/imgs/blackdude.jpeg" alt="" 
                                    class=" w-[2em] h-[2em] object-cover rounded-full max-w-full align-middle inline-block snippit-avtar"
                                    >
                                </div>
                                <div class="fifth">
                                    <div class="w-[1.5em] h-[1.5em] bg-accent text-white rounded-full flex justify-center items-center font-[.75em]">
                                        <Icon icon="material-symbols:check" />
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-sm">
                    <h5 class=" text-titles-links tracking-[-.025em] font-bold text-[1.25em] leading-[1.2]">Speed</h5>
                    <div class=" opacity-[.6] font-semibold">
                        <p>
                            100+ datacenters worldwide means your site loads fast for every visitor.
                        </p>
                    </div>
                </div>
            </div>
        </div>

        <div  class=" slack-wrapper mt-10">
            <div ref="card3" class="animation card-3 card-body bg-neutral-800 w-[330px] h-[360px] rounded-lg mx-auto p-5">
                <h4 class="card-body__heading text-titles-links tracking-[-.025em] text-[1.5em] font-bold leading-[1.2]">03.</h4>
                <div class=" bg-neutral-800 rounded-[.5em] overflow-hidden ">
                    <div class=" w-[85%]  h-[96px]   rounded-md mx-auto my-[2.75em] ">
                        <div class="snippet__body flex flex-col justify-center items-center min-h-[6em] rounded-[.375em] p-[.75em] bg-neutral-700 ">
                            <div class="w-full flex-1 ">
                                <div class="switch-wrapper">
                                    <div class="snippit-switch">
                                        <img class="switch-img w-[1em] max-w-full align-middle inline-block" src="/assets/imgs/slack.svg" alt="" >
                                        <div class="snippit-switch-text leading-[1.25] tracking-[-.005em] text-[.975em] ">
                                            <p>Slack Channel</p>
                                        </div>
                                        <div class=" w-[2.5em] h-[1.2em] bg-accent rounded-full py-1 px-[3px] flex justify-end items-center">
                                            <div class=" w-[.75em] h-[.75em] bg-white rounded-full"></div>
                                        </div>
                                    </div>
                                <div class=" w-full h-[1px] bg-neutral-600">
                                </div>
                                <div class="snippit-switch">
                                        <img class="switch-img w-[1.1em] max-w-full align-middle inline-block" src="/assets/imgs/evernote.svg" alt="" >
                                        <div class="snippit-switch-text leading-[1.25] tracking-[-.005em] text-[.975em]">
                                            <p>Evernote</p>
                                        </div>
                                        <div class=" w-[2.5em] h-[1.2em] rounded-full py-1 px-[3px] flex justify-start items-center bg-neutral-600">
                                            <div class=" w-[.75em] h-[.75em] bg-white rounded-full"></div>
                                        </div>
                                    </div>
                            </div>
                        </div>
                        </div>
                    </div>
                </div>
                <div class="col-sm">
                    <h5 class=" text-titles-links tracking-[-.025em] font-bold text-[1.25em] leading-[1.2]">Security</h5>
                    <div class=" opacity-[.6] font-semibold">
                        <p>
                            Built-in SSL for all sites, and no need to manage or update risk-prone plugins.
                        </p>
                    </div>
                </div>
            </div>
        </div>

</template>



<style scoped>

.col-sm {
    grid-column-gap: .5em;
    grid-row-gap: .5em;
    grid-template-rows: auto;
    grid-template-columns: 1fr;
    grid-auto-columns: 1fr;
    justify-items: start;
    display: grid;
}
.snippet__body{
    box-shadow: 0 0 0 1.5px var(--neutral-800), 0 0 0 3px var(--neutral-700);
    
}

.dot-list {
    display: grid;
    grid-template-columns: repeat(12,1fr);
    grid-template-rows: auto;
    gap: .75em;
}

.dot {
    grid-area: span 1/ span 1 / span 1 / span 1;
}

.snippt-block {
    display: grid;
    width: 100%;
    grid-column-gap: 2px;
    grid-row-gap: 2px;
    grid-template-rows: auto;
    grid-template-columns: 1fr auto;
    grid-auto-columns: auto;
    grid-auto-flow: column;
    align-items: center;
}

.block-copy {
    background-image: linear-gradient(270deg, var(--neutral-600) 2%, rgba(48, 54, 61, 0));
    color: var(--titles-links);
    text-align: center;
    text-transform: none;
    border-radius: .25em;
    font-family: ICONS SHARP, sans-serif;
    font-size: 1.5em;
    font-weight: 400;
    line-height: 2;
    position: relative;
    min-width: 2em;
}

.block-copy__icon {
    z-index: 1;
    min-width: 2em;
    background-color: var(--primary);
    color: var(--titles-links);
    text-align: center;
    text-transform: none;
    font-size: 1.125em;
    font-weight: 400;
    line-height: 2;
    position: relative;
    box-shadow: 0 12px 24px -12px #000;
}
.avatar-wrap {
    display: grid;
    grid-template-columns: auto .5fr;
    grid-template-rows: auto;
    gap: 1em .75em;
    align-items: center;
}

.first {
    grid-column: 1/3;
}

.sec {
    grid-column: 1/2;
    grid-row: 2/3;
}

.thi {
    grid-column: 2/3;
    grid-row: 2/3;
}

.forth {
    grid-column: 1/2;
    grid-row: 3/4;
    
}

.fifth {
    grid-column: 2/3;
    grid-row: 3/4;
    justify-self: end;
}


.snippit-avtar {
    box-shadow: 0 0 0 2.5px var(--neutral-700);
    margin-left: -.5em;
}

.switch-wrapper {
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: auto;
  gap: 8px;
}
.snippit-switch {
    display: grid;
    grid-template-columns: auto 1fr auto;
    grid-template-rows: auto;
    gap: 4px 16px;
    align-items: center;
}

.switch-img {
    grid-column: 1/2;
    grid-row: 1/2;
}

.snippit-switch .snippit-switch-text {
    justify-self: start;
}


.image-bg-cover {
    filter: grayscale();
    mix-blend-mode: multiply;
}

/* @keyframes slide-fade-in {
    from {
        opacity: 0;
        transform: translateY(5vh);
    }
}

@media (prefers-reduced-motion: no-preference) {
    .card-1 {
        view-timeline-name: --item-timeline;
        animation: slide-fade-in 0s both;
        animation-timeline: --item-timeline;
        animation-range: contain 0% contain 50%;
    }
    .card-2 {
        view-timeline-name: --item-timeline;
        animation: slide-fade-in 1s both;
        animation-timeline: --item-timeline;
        animation-range: contain 0% contain 50%;
    }
    .card-3 {
        view-timeline-name: --item-timeline;
        animation: slide-fade-in 2.5s both;
        animation-timeline: --item-timeline;
        animation-range: contain 0% contain 50%;
    }
} */
</style>