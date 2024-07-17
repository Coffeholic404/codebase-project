<script setup>
import { Icon } from "@iconify/vue";
const { $gsap } = useNuxtApp();

const one = ref(null);
  const two = ref(null);
  const three = ref(null);
  const four = ref(null);
  const five = ref(null);

onMounted(()=> {
    const cards = [one, two, three, four, five];
  cards.forEach((card, index) => {
    $gsap.fromTo(card.value, 
      { opacity: 0, x: 0 }, 
      { 
        opacity: 1, 
        x: 1232,
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
    <div class="process-steps">
        <div ref="one" class="process-steps-step z-[5] w-full flex items-center relative -left-[77rem]">
            <div class="process-steps-indicator">
                <div class="process-steps-indicator-icon"><Icon icon="material-symbols:check" /></div>
            </div>
            <div class="process-steps-item rounded-xs fade-in-on-scroll"
            >
                <div class="process-margin mb-[1.75em]">
                    <div class="process-caption-holder z-[5] w-full">
                        <div class="process-row-sm">
                            <div class="caption">Step</div>
                            <div class="caption opacity-[.5]">01</div>
                        </div>
                        <div  class="line-holder col-span-1 row-span-1 w-full relative">
                            <div  class="process-line-animated"
                                style="width: 100%; height: 1px;"></div>
                        </div>
                    </div>
                </div>
                <div class="process-margin-xs mb-[.5em]">
                    <h3 class=" text-titles-links relative font-bold text-[1.875em] process-title">Build with raw ingredients</h3>
                </div>
                <div>Drag in unstyled HTML elements for full control, or use pre-built pieces for complex elements like
                    sliders, tabs, background videos, and more.<br></div>
            </div>
        </div>

        <div ref="two" class="process-steps-step z-[5] w-full flex items-center relative -left-[77rem]">
            <div class="process-steps-indicator">
                <div class="process-steps-indicator-icon"><Icon icon="material-symbols:check" /></div>
            </div>
            <div class="process-steps-item rounded-xs fade-in-on-scroll"
            >
                <div class="process-margin mb-[1.75em]">
                    <div class="process-caption-holder z-[5] w-full">
                        <div class="process-row-sm">
                            <div class="caption">Step</div>
                            <div class="caption opacity-[.5]">01</div>
                        </div>
                        <div  class="line-holder col-span-1 row-span-1 w-full relative">
                            <div  class="process-line-animated"
                                style="width: 100%; height: 1px;"></div>
                        </div>
                    </div>
                </div>
                <div class="process-margin-xs mb-[.5em]">
                    <h3 class=" text-titles-links relative font-bold text-[1.875em] process-title">Build with raw ingredients</h3>
                </div>
                <div>Drag in unstyled HTML elements for full control, or use pre-built pieces for complex elements like
                    sliders, tabs, background videos, and more.<br></div>
            </div>
        </div>

        <div ref="three" class="process-steps-step z-[5] w-full flex items-center relative -left-[77rem]">
            <div class="process-steps-indicator">
                <div class="process-steps-indicator-icon"><Icon icon="material-symbols:check" /></div>
            </div>
            <div class="process-steps-item rounded-xs fade-in-on-scroll"
            >
                <div class="process-margin mb-[1.75em]">
                    <div class="process-caption-holder z-[5] w-full">
                        <div class="process-row-sm">
                            <div class="caption">Step</div>
                            <div class="caption opacity-[.5]">01</div>
                        </div>
                        <div  class="line-holder col-span-1 row-span-1 w-full relative">
                            <div  class="process-line-animated"
                                style="width: 100%; height: 1px;"></div>
                        </div>
                    </div>
                </div>
                <div class="process-margin-xs mb-[.5em]">
                    <h3 class=" text-titles-links relative font-bold text-[1.875em] process-title">Build with raw ingredients</h3>
                </div>
                <div>Drag in unstyled HTML elements for full control, or use pre-built pieces for complex elements like
                    sliders, tabs, background videos, and more.<br></div>
            </div>
        </div>

        <div ref="four" class="process-steps-step z-[5] w-full flex items-center relative -left-[77rem]">
            <div class="process-steps-indicator">
                <div class="process-steps-indicator-icon"><Icon icon="material-symbols:check" /></div>
            </div>
            <div class="process-steps-item rounded-xs fade-in-on-scroll"
            >
                <div class="process-margin mb-[1.75em]">
                    <div class="process-caption-holder z-[5] w-full">
                        <div class="process-row-sm">
                            <div class="caption">Step</div>
                            <div class="caption opacity-[.5]">01</div>
                        </div>
                        <div  class="line-holder col-span-1 row-span-1 w-full relative">
                            <div  class="process-line-animated"
                                style="width: 100%; height: 1px;"></div>
                        </div>
                    </div>
                </div>
                <div class="process-margin-xs mb-[.5em]">
                    <h3 class=" text-titles-links relative font-bold text-[1.875em] process-title">Build with raw ingredients</h3>
                </div>
                <div>Drag in unstyled HTML elements for full control, or use pre-built pieces for complex elements like
                    sliders, tabs, background videos, and more.<br></div>
            </div>
        </div>

        <div ref="five" class="process-steps-step z-[5] w-full flex items-center relative -left-[77rem]">
            <div class="process-steps-indicator">
                <div class="process-steps-indicator-icon"><Icon icon="material-symbols:check" /></div>
            </div>
            <div class="process-steps-item rounded-xs fade-in-on-scroll"
            >
                <div class="process-margin mb-[1.75em]">
                    <div class="process-caption-holder z-[5] w-full">
                        <div class="process-row-sm">
                            <div class="caption">Step</div>
                            <div class="caption opacity-[.5]">01</div>
                        </div>
                        <div  class="line-holder col-span-1 row-span-1 w-full relative">
                            <div  class="process-line-animated"
                                style="width: 100%; height: 1px;"></div>
                        </div>
                    </div>
                </div>
                <div class="process-margin-xs mb-[.5em]">
                    <h3 class=" text-titles-links relative font-bold text-[1.875em] process-title">Build with raw ingredients</h3>
                </div>
                <div>Drag in unstyled HTML elements for full control, or use pre-built pieces for complex elements like
                    sliders, tabs, background videos, and more.<br></div>
            </div>
        </div>

        <!-- <div class="process-steps-way-bg  w-[2px] absolute left-[1.5em] right-auto overflow-hidden">
            <div class="process-steps-way w-full bg-indigo-900 absolute top-0 bottom-auto left-0 right-0" style="will-change: width, height; height: 27.6%;"></div>
        </div>  -->
    </div>
</template>



<style scoped>
.process-steps {
    display: grid;
    grid-column-gap: 2.5em;
    grid-row-gap: 2.5em;
    grid-template-rows: auto;
    grid-template-columns: 1fr;
    justify-items: center;
    padding-top: 5em;
    padding-bottom: 5em;
    position: relative;
}

.process-steps-indicator {
    width: 3em;
    height: 3em;
    border: 5px solid var(--indigo-900);
    background-color: var(--indigo-600);
    outline-color: var(--background);
    outline-offset: 0px;
    border-radius: 9999px;
    outline-width: 10px;
    outline-style: solid;
    justify-content: center;
    align-items: center;
    margin-top: 2em;
    display: flex;
}

.process-steps-indicator-icon {
    color: var(--white);
    font-family: ICONS SHARP, sans-serif;
    font-size: 1.5em;
    line-height: 1;
}

.process-steps-item {
    background-color: var(--neutral-800);
    flex: 1;
    margin-left: 2em;
    padding: 3em;
}

.rounded-xs {
    border-radius: .5em;
    position: relative;
    overflow: hidden;
}

.process-caption-holder {
    display: grid;
    gap: 1em;
    grid-template-rows: auto;
    grid-template-columns: auto 1fr;
    grid-auto-columns: 1fr;
    align-items: center;
    position: relative;
}

.process-row-sm {
    display: grid;
    gap: .5em;
    grid-template-rows: auto;
    grid-template-columns: auto;
    grid-auto-columns: auto;
    grid-auto-flow: column;
    justify-content: start;
}

.caption {
    letter-spacing: .1em;
    text-transform: uppercase;
    font-size: .625em;
    font-weight: 600;
}

.process-line-animated {
    width: 100%;
    height: 1px;
    background-image: linear-gradient(to right, var(--border), rgba(33, 38, 45, 0));
    position: absolute;
    top: 0%;
    bottom: auto;
    left: 0%;
    right: 0%;
}

.process-title {
    letter-spacing: -.025em;
    line-height: 1.2;
}


@media (max-width: 479px) {
    .process-steps-indicator {
        width: 2.5em;
        height: 2.5em;
        margin-top: 1.25em;
    }

    .process-steps-item {
        margin-left: 1em;
        padding-left: 1.5em;
        padding-right: 1.5em;
    }

    .process-margin {
        margin-inline: 0;
        margin-top: 0;
        margin-bottom: 1.375em;
    }

    .process-margin-xs{
        margin-inline: 0;
        margin-top: 0;
    }
}

@media (min-width: 500px) and (max-width: 767px) {
    .process-steps-indicator {
        margin-top: 1em;
    }
    .process-steps-indicator-icon {
        font-size: 1em;
    }

    .process-steps-item {
        padding-top: 2em;
        padding-bottom: 2em;
    }

    .process-margin {
        margin-inline: 0;
        margin-top: 0;
        margin-bottom: 1.5em;
    }

    .process-margin-xs{
        margin-inline: 0;
        margin-top: 0;
        margin-bottom: .375em;
    }

    h3 {
        font-size: 1.5em;
    }
}

@media (min-width: 768px) and (max-width: 991px) {
    .process-margin {
        margin-inline: 0;
        margin-top: 0;
        margin-bottom: 1.625em;
    }

    .process-margin-xs{
        margin-inline: 0;
        margin-top: 0;
    }
}
</style>