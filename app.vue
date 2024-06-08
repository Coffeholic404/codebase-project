<script setup>
import { Icon } from "@iconify/vue";
</script>

<template>
  <div>

    <div class="nav__wrapper relative">
      <TheNavbar />
    </div>
    <div>
      <div class="wrapper py-[9em] ">
        <div class="w-full py-[5em] h-full wrapper__continer">
          <div class="w-full max-w-[48em] mx-auto px-[1.25em]">
            <div class="">
              <h2 class="title__sm  text-[3em] text-titles-links  font-bold text-center">Get help from hundred of web <a
                  class=" text-primary" href="#">sections</a>, and ready-to-use <a class=" text-primary"
                  href="#">templates</a> to grow your business.</h2>
              <div class="start__wrapper mt-8">
                <div class="rating__stars ">
                  <div>
                    <Icon icon="material-symbols:star-rounded" class="text-yellow-300 w-6 h-8 text-2xl" />
                  </div>
                  <div>
                    <Icon icon="material-symbols:star-rounded" class="text-yellow-300 w-6 h-8 text-2xl" />
                  </div>
                  <div>
                    <Icon icon="material-symbols:star-rounded" class="text-yellow-300 w-6 h-8 text-2xl" />
                  </div>
                  <div>
                    <Icon icon="material-symbols:star-rounded" class="text-yellow-300 w-6 h-8 text-2xl" />
                  </div>
                  <div>
                    <Icon icon="material-symbols:star-rounded" class="text-yellow-300 w-6 h-8 text-2xl" />
                  </div>
                </div>
                <h6 class="start__wrapper--heading text-titles-links text-center">Loved by teams worldwide</h6>
                <div class=" start__wrapper--subheading font-medium text-xs text-center">99.9% of them think Codebase is
                  great</div>
              </div>
            </div>
            <div class="sigh__wrapper w-full max-w-[24em] mx-auto text-center justify-center items-center  mt-8">
              <form>
                <div class="flex flex-col gap-[1.2px] basis-[380px] flex-1 my-4 relative">
                  <div class="input input__email h-[3.5em]  bg-neutral-800 border-1 border-[#000]  relative">
                    <input type="text" name="" id="" placeholder="Work Email"
                      class="  bg-neutral-800  text-titles-links w-full h-full">
                    <div class=" absolute top-4 left-3">
                      <Icon icon="ic:baseline-email" class="w-[12px] h-[12px] text-slate-500" />
                    </div>
                  </div>
                  <div class="input input__password h-[3.5em]  bg-neutral-800 border-1 border-[#000]  relative">
                    <input type="password" name="" id="" placeholder="Password 8+ characters"
                      class="  bg-neutral-800  text-titles-links w-full h-full">
                    <div class=" absolute top-4 left-3">
                      <Icon icon="material-symbols:lock" class="w-[12px] h-[12px] text-slate-500" />
                    </div>
                  </div>
                </div>
                <button
                  class="button text-white bg-primary py-[.75em] px-[1.25em] rounded-2xl font-semibold text-lg">Sign
                  Up</button>
                <div class="flex flex-col justify-center items-center gap-4 mt-4">
                  <p class="caption">Or sign up with:</p>
                  <div class="flex gap-4">
                    <a href=""><img src="/assets/imgs/google.svg" alt=""></a>
                    <a href=""><img src="/assets/imgs/Facebook.svg" alt=""></a>
                    <a href=""><img src="/assets/imgs/vk.svg" alt=""></a>
                    <a href=""><img src="/assets/imgs/linkedin.svg" alt=""></a>
                    <a href=""><img src="/assets/imgs/slack.svg" alt=""></a>
                  </div>
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>

    </div>
    <div class=" bg-hero-pattern  w-full min-h-[100dvh]">
      <TheSeo />
    </div>
  </div>

  <article class=" min-h-[100dvh] w-full py-[5em] relative">
    <div class="sec-bg w-full h-full flex justify-center items-center absolute top-0 right-0 left-0 bottom-0">
      <img
        src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d7639a8f711_bg-shape-08.png"
        loading="lazy"
        srcset="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d7639a8f711_bg-shape-08-p-500.png 500w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d7639a8f711_bg-shape-08-p-800.png 800w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d7639a8f711_bg-shape-08-p-1080.png 1080w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d7639a8f711_bg-shape-08-p-1600.png 1600w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d7639a8f711_bg-shape-08-p-2000.png 2000w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d7639a8f711_bg-shape-08-p-2600.png 2600w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d7639a8f711_bg-shape-08.png 3200w"
        alt="" sizes="100vw" class="bg-pattern-image">
    </div>
    <div class="sec-wrapper z-[5] w-full max-w-[64em] mx-auto px-[1.25em] relative">
      <div class="side-by-side-list w-full max-w-[]">
        <Feature />
        <Feature2 />
      </div>
    </div>
  </article>

  <article class="banner-section min-h-[100dvh] py-[10em] rounded-[.5em] bg-teal-700 w-full">
    <div class="banner-card-wrapper w-full max-w-[56em]   px-[1.25em] mx-auto rounded-[.5em] z-[10000]">
      <div class="banner-card relative rounded-[.5em]  p-[4em]">
        <img
          src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949dbfc1a8f6cf_Rectangle-23.jpg"
          loading="lazy"
          srcset="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949dbfc1a8f6cf_Rectangle-23-p-500.jpeg 500w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949dbfc1a8f6cf_Rectangle-23-p-800.jpeg 800w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949dbfc1a8f6cf_Rectangle-23.jpg 1024w"
          alt="" sizes="(max-width: 479px) 92vw, (max-width: 991px) 95vw, 856px"
          class="image-background z-[5] w-full max-w-full h-full filter-none object-cover absolute top-0 bottom-0 right-0 left-0 align-middle inline-block rounded-[.5em]">

        <img
          src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d339fa8f555_photo-1616587226830-e493599b0c15.jpeg"
          loading="lazy" alt=""
          class="image-bg-cover opacity-[.15] z-[5] w-full max-w-full h-full object-cover absolute top-0 bottom-0 right-0 left-0 align-middle inline-block rounded-[.5em]">


        <div class="w-layout-grid column-md content-centered banner-content-centered w-full text-center mx-auto items-center relative z-[5]" >
          <div class="banner-max-width-lg">
            <div class="content-left text-left">
              <div class="banner-title-xs  text-white z-[5] font-extrabold leading-[1.1] relative">“Best templates and support out there! They are always happy to
                help with any issues you may be having”</div>

              <div class="banner-margin-vertical margin-2xl mx-0 my-[2em]">
                <div class="banner-row-sm">
                  <img
                    src="/assets/imgs/stack_overflow.svg"
                    loading="lazy" alt="" class="client-logo-base align-middle inline-block">
                  <div class="banner-text-sm text-white relative">
                    <div>George Light</div>
                    <div>Business Director, Stack</div>
                  </div>
                </div>
              </div>

              <div class="banner-stats-3 text-white relative">
                <div class="banner-content-left flex flex-col text-left relative">
                  <div class="banner-row-sm items-center">
                    <div class="banner-text-xl">
                      <div class="material-icons"><Icon icon="material-symbols:data-exploration" /></div>
                    </div>
                    <h5>73%</h5>
                  </div>
                  <div class="text-xs leading-tighter">Time to achieve the first results</div>
                </div>
                <div class="banner-content-left flex flex-col text-left relative">
                  <div class="banner-row-sm items-center">
                    <div class="banner-text-xl">
                      <div class="material-icons"><Icon icon="material-symbols:verified" /></div>
                    </div>
                    <h5>73%</h5>
                  </div>
                  <div class="text-xs leading-tighter">Time to achieve the first results</div>
                </div>
                <div class="banner-content-left flex flex-col text-left relative">
                  <div class="banner-row-sm items-center">
                    <div class="banner-text-xl">
                      <div class="material-icons">
                        <Icon icon="material-symbols:history" />
                      </div>
                    </div>
                    <h5>73%</h5>
                  </div>
                  <div class="text-xs leading-tighter">Time to achieve the first results</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class=" w-full h-[50%] absolute top-auto bottom-0 left-0 right-0 bg-neutral-800 z-[0]"></div>
  </article>

  <article class=" relative overflow-hidden w-full">
    <FeatureTwo />
  </article>

  <article class="feature3-wrapper w-full min-h-[100dvh] py-[5em] bg-amber-900">
      <FeatureThree />
  </article>
</template>

<style scoped>

.nav__wrapper{
  position: sticky;
  top: 0;
  right: 0;
  left: 0;
  z-index: 1001;
}


.wrapper {
  /* position: absolute; */
  width: 100%;
  top: 0;
  left: 0;
  /* min-height: 100dvh; */
  background-image: radial-gradient(circle farthest-corner at -25% -50%, var(--background) 36%, rgba(13, 17, 23, 0) 48%), 
  radial-gradient(circle farthest-corner at -25% 150%, var(--background) 45%, rgba(13, 17, 23, 0) 89%), 
  radial-gradient(circle farthest-corner at -25% -100%, rgba(13, 17, 23, 0) 55%, rgba(13, 17, 23, .28) 65%, rgba(13, 17, 23, 0) 68%), 
  radial-gradient(circle farthest-corner at -33% -75%, #1f00cc 48%, rgba(131, 5, 49, 0) 56%), 
  radial-gradient(circle farthest-side at 0% -50%, rgba(13, 17, 23, 0) 64%, rgba(1, 2, 36, .4) 69%, rgba(13, 17, 23, 0) 81%), 
  radial-gradient(circle farthest-corner at 0% -50%, rgba(13, 17, 23, 0) 33%, #010c5f 51%, rgba(13, 17, 23, 0) 72%);
  border-radius: 1px;
}

.title__sm {
  letter-spacing: -.04em;
  line-height: 1.1;
}

@media (max-width: 991px) {
  .title__sm {
    font-size: 2.5em;
  }
}

.wrapper__continer {
  background-image: url(/assets/imgs/bg-shape-001-p-2000.png);
  background-size: cover;
  background-position: top 30% left 10%;
  background-repeat: no-repeat;
}

.start__wrapper {
  grid-row: 2/3;
  display: grid;
  gap: .25em;
  grid-template-rows: auto;
  grid-template-columns: 1fr;
  grid-auto-columns: 1fr;
  justify-items: center;
  align-self: end;
}

.rating__stars {
  /* display: flex;
  gap: 0; */
  display: grid;
  grid-column-gap: 0px;
  grid-row-gap: 0px;
  grid-template-rows: auto;
  grid-template-columns: auto;
  grid-auto-columns: auto;
  grid-auto-flow: column;
}

.start__wrapper--heading {
  letter-spacing: -.025em;
  font-size: 1em;
  font-weight: 600;
  line-height: 1.2;
}
.button {
  line-height: 1;
  transition: background-color .3s, opacity .3s, box-shadow .3s, color .3s;
  
}

.button:hover {
  box-shadow: inset 0 0 200px 200px rgba(0, 0, 0, .15);
}
.sigh__wrapper{
    grid-column-gap: 1em;
    grid-row-gap: 1em;
    grid-template-rows: auto;
    grid-template-columns: 1fr;
    grid-auto-columns: 1fr;
    display: grid;
    /* position: relative; */
}

.input{
    padding: 0 1.125em 0 3em;
    font-size: 80%;
    font-weight: 400;
    line-height: 1;
    transition: background-color .25s, box-shadow .25s;

    box-shadow: inset 0 0 0 1px transparent;
}

.input__email {
  border-top-left-radius: .5em;
    border-top-right-radius: .5em;
}

.input__password {
  border-bottom-left-radius: .5em;
    border-bottom-right-radius: .5em;
}
.caption {
  letter-spacing: .1em;
    text-transform: uppercase;
    font-size: .625em;
    font-weight: 600;
}

.side-by-side-list {
    display: grid;
    z-index: 5;
    grid-column-gap: 5em;
    grid-row-gap: 5em;
    grid-template-rows: auto;
    grid-template-columns: 1fr;
    position: relative;
}

/* .banner{
  background-image: linear-gradient(to top, var(--background), rgba(13, 17, 23, 0) 15%), linear-gradient(to bottom, var(--background), rgba(13, 17, 23, 0) 15%), radial-gradient(circle farthest-side at 50% 0%, rgba(13, 17, 23, 0), var(--background)), url(https://assets-global.website-files.com/6239c2c…/6239c2c…_bg-tile-dark.svg);
    background-position: 0 0, 0 0, 0 0, -1px -1px;
    background-size: auto, auto, auto, 64px;
    position: relative;
} */

.container-md {
    z-index: 5;
    width: 100%;
    max-width: 56em;
    margin-left: auto;
    margin-right: auto;
    padding-left: 1.25em;
    padding-right: 1.25em;
    position: relative;
}

/* .image-background {
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
} */

/* img {
    max-width: 100%;
    vertical-align: middle;
    display: inline-block;
} */

/* .opacity-15 {
    opacity: .15;
}
.image-bg-cover {
    z-index: 0;
    width: 100%;
    height: 100%;
    filter: grayscale();
    mix-blend-mode: multiply;
    object-fit: cover;
    position: absolute;
    top: 0%;
    bottom: 0%;
    left: 0%;
    right: 0%;
} */

.column-md.content-centered {
    grid-column-gap: 1.5em;
    grid-row-gap: 1.5em;
    grid-template-rows: auto;
    grid-template-columns: 1fr;
    grid-auto-columns: 1fr;
    justify-items: center;
    display: grid;
}
.content-centered {
    width: 100%;
    text-align: center;
    flex-direction: column;
    align-items: center;
    margin-left: auto;
    margin-right: auto;
    display: flex;
    position: relative;
}

.column-md {
    grid-column-gap: 1.5em;
    grid-row-gap: 1.5em;
    grid-template-rows: auto;
    grid-template-columns: 1fr;
    grid-auto-columns: 1fr;
    justify-items: start;
    display: grid;
}

.w-layout-grid {
    grid-row-gap: 16px;
    grid-column-gap: 16px;
    grid-template-rows: auto auto;
    grid-template-columns: 1fr 1fr;
    grid-auto-columns: 1fr;
    display: grid;
}

.row-sm {
    grid-column-gap: .5em;
    grid-row-gap: .5em;
    grid-template-rows: auto;
    grid-template-columns: auto;
    grid-auto-columns: auto;
    grid-auto-flow: column;
    justify-content: start;
    display: grid;
}

.stats-3-column-sm {
    grid-column-gap: 1em;
    grid-row-gap: 1em;
    grid-template-rows: auto;
    grid-template-columns: auto auto auto;
}

.material-icons {
    text-transform: none;
    font-family: ICONS FILLED, sans-serif;
}

h5 {
    letter-spacing: 0;
    margin-top: 0;
    margin-bottom: 0;
    font-size: 1.25em;
    font-weight: 700;
    line-height: 1.2;
}

.banner-content-centered {
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: auto;
    justify-content: center;
    align-items: center;
    grid-auto-columns: 1fr;
    gap: 1.5em;
}

.banner-max-width-lg {
    grid-area: span 1 / span 1 / span 1 / span 1;
    width: 100%;
    max-width: 32em;
}

.content-left {
    text-align: left;
    flex-direction: column;
    align-items: flex-start;
    display: flex;
}

.banner-title-xs {
    font-size: 2.5em;
    letter-spacing: -.03em;
}

.banner-row-sm {
    display: grid;
    grid-template-rows: auto;
    grid-template-columns: auto;
    grid-auto-columns: auto;
    grid-auto-flow: column;
    justify-content: start;
    gap: .5em;
}

.client-logo-base {
    height: 2em;
    max-width: 6em;
}

.banner-text-sm {
    line-height: 1;
    letter-spacing: -.005em;
    font-size: .875em;
}

.banner-stats-3 {
    display: grid;
    grid-column-gap: 1em;
    grid-row-gap: 1em;
    grid-template-rows: auto;
    grid-template-columns: auto auto auto;
    grid-auto-columns: 1fr;
}

.banner-text-xl {
    letter-spacing: -.01em;
    font-size: 1.5em;
}

.feature3-wrapper {
  background-image: linear-gradient(to top, var(--background), rgba(13, 17, 23, 0) 15%), linear-gradient(to bottom, var(--background), rgba(13, 17, 23, 0) 15%), radial-gradient(circle farthest-side at 50% 0%, rgba(13, 17, 23, 0), var(--background)), url(/assets/imgs/bg-tile-dark.svg);
    background-position: 0 0, 0 0, 0 0, -1px -1px;
    background-size: auto, auto, auto, 64px;
    position: relative;
}

@media (max-width: 479px) {
  .title__sm {
    font-size: 1.75em;
  }

  .title-lg {
        letter-spacing: -.01em;
        font-size: 1.875em;
    }

  .padding-6xl {
        padding: 2.5em 1.5em; 
    }
    .stats-3-column-sm {
        width: 100%;
        grid-column-gap: .5em;
        grid-row-gap: .5em;
        grid-template-columns: auto;
    }
    .title-xs {
        font-size: 1.75em ;
    }

    .banner{
      padding:1rem;
    }
    .banner-title-xs {
    font-size: 1.75em !important;
  }
  .banner-margin-vertical {
    margin: 1.625em 0 !important;
  }

  .banner-stats-3{
    width: 100%;
    gap: .5em;
    grid-template-columns: auto;
  }
}

@media (max-width: 767px) {
  .padding-6xl {
        padding: 3em; 
    }

    .banner-title-xs {
    font-size: 2.125em;
  }

  .banner-margin-vertical{
    margin: 1.75em 0;
  } 
}

@media (max-width: 991px) {
  .padding-6xl {
        padding: 3.5em; 
    }

    .banner-title-xs {
    font-size: 2.25em;
  }

  .banner-margin-vertical{
    margin: 1.875em 0;
  } 
}


</style>
