<script setup>
const { $gsap } = useNuxtApp();
const img = ref(null);

onMounted(() => {
    $gsap.fromTo(img.value, 
    { opacity: 0, y: 50}, 
    { 
      opacity: 1, 
      y: 0,
      delay:1,
      easy: "power2.inout",
      scrollTrigger: {
        trigger: img.value,
        start: 'top 50%', // Adjust based on when you want the animation to start
        end: 'top 50%',
        scrub: false,
        toggleActions: 'play none none none',
      },
    });
});
</script>

<template>
    <div class="container-lg z-[5] w-full max-w-[64em] mx-auto p-[1.25em] relative">
        <div  class="footer-grid">

            <div ref="img" class="footer-1-cta-box z-[5] bg-primary text-center rounded-[.5em] mt-[-4em] mb-[3em] py-[4em] px-[6em] overflow-hidden flex flex-col justify-center items-center">
                <div class="footer-1-cta-grid">
                    <h2 class="cta-title-sm text-white col-span-1 row-span-1">Move
                        even faster with <span class="logo-inside-text">Norman</span> UI Kit for Webflow.</h2>
                    <div class="cta-row-base">
                        <a href="/"
                            class="button-animated cta-button bg-blue-800 self-center justify-self-end z-[5] text-white text-center rounded-full py-[.75em] px-[1.25em] text-[1.125em] font-semibold leading-[1] overflow-hidden relative flex items-center justify-center max-w-full">
                            <div class="button-label z-[5] relative flex justify-center items-center">Take the Tour
                            </div>
                            <div class="button-hover-background">
                            </div>
                        </a><a href="https://webflow.com/templates/html/codebase-it-company-website-template"
                            target="_blank"
                            class="button-animated cta-button bg-blue-500 self-center justify-self-end z-[5] text-white text-center rounded-full py-[.75em] px-[1.25em] text-[1.125em] font-semibold leading-[1] overflow-hidden relative flex items-center justify-center max-w-full">
                            <div class="button-label z-[5] relative flex justify-center items-center">Browse in Webflow
                            </div>
                            <div class="button-hover-background">
                            </div>
                        </a>
                </div>
                </div>



                <div
                    class="bg-pattern-wrap w-full h-full flex items-start justify-center absolute top-0 bottom-0 left-0 right-0">
                    <img src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d39c0a8f70c_bg-shape-05.png"
                        loading="lazy" sizes="(max-width: 479px) 92vw, (max-width: 767px) 95vw, 96vw"
                        srcset="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d39c0a8f70c_bg-shape-05-p-500.png 500w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d39c0a8f70c_bg-shape-05-p-800.png 800w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d39c0a8f70c_bg-shape-05-p-1080.png 1080w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d39c0a8f70c_bg-shape-05-p-1600.png 1600w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d39c0a8f70c_bg-shape-05-p-2000.png 2000w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d39c0a8f70c_bg-shape-05-p-2600.png 2600w, https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d39c0a8f70c_bg-shape-05.png 3200w"
                        alt=""
                        class="bg-pattern-image w-full h-full object-cover my-auto absolute top-auto bottom-auto left-0 right-0 max-w-full align-middle inline-block">
                </div>
            </div>

            <div class="footer-1-main-grid">
                <a href="/"
                    class="footer-1-logo w-inline-block col-span-1 row-span-1 w-[8em] max-w-full inline-block"><img
                        src="https://assets-global.website-files.com/6239c2cd52949d0f76a8f421/6239c2ce52949d9cd4a8f705_logo_white.svg"
                        loading="lazy" alt="" class="image-contain "></a>
                <div class=" col-span-1 row-span-1">
                    <div class="footer-1-sub-grid">
                        <div class="column-sm">
                            <div class="margin-3 col-span-1 row-span-1">
                                <h6 class="footer-1-nav-heading">Product Tours</h6>
                            </div><a href="/product-tour/home-1"
                                class="footer-1-link-gray col-span-1 row-span-1">Product Tour 1</a><a
                                href="/product-tour/home-2" class="footer-1-link-gray col-span-1 row-span-1">Product
                                Tour 2</a><a href="/product-tour/home-3" aria-current="page"
                                class="footer-1-link-gray col-span-1 row-span-1 w--current">Product Tour 3</a><a
                                href="/product-tour/home-4" class="footer-1-link-gray col-span-1">Product Tour 4</a><a
                                href="/product-tour/home-5" class="footer-1-link-gray col-span-1 row-span-1">Product
                                Tour 5</a>
                        </div>

                        <div class="column-sm">
                            <div class="margin-3 col-span-1 row-span-1">
                                <h6 class="footer-1-nav-heading">Product </h6>
                            </div><a href="/product/pricing-1" class="footer-1-link-gray col-span-1 row-span-1">Pricing
                                1</a><a href="/product/pricing-2"
                                class="footer-1-link-gray col-span-1 row-span-1">Pricing 2</a><a
                                href="/product/pricing-3" class="footer-1-link-gray col-span-1 row-span-1">Pricing
                                3</a><a href="/product/customer"
                                class="footer-1-link-gray col-span-1 row-span-1">Customer</a><a
                                href="https://codebase-template.webflow.io/customer-story/petsplay"
                                class="footer-1-link-gray col-span-1 row-span-1">Customer Detail</a><a
                                href="/product/faq" class="footer-1-link-gray col-span-1 row-span-1">FAQ</a><a
                                href="/product/download" class="footer-1-link-gray col-span-1 row-span-1">Download</a>
                        </div>

                        <div class="column-sm">
                            <div class="margin-bottom margin-3 col-span-1 row-span-1">
                                <h6 class="footer-1-nav-heading">Company</h6>
                            </div><a href="/company/about-us-1" class="footer-1-link-gray col-span-1 row-span-1">About
                                1</a><a href="/company/about-us-2"
                                class="footer-1-link-gray col-span-1 row-span-1">About 2</a><a
                                href="/company/about-us-3" class="footer-1-link-gra col-span-1 row-span-1y">About
                                3</a><a href="https://codebase-template.webflow.io/team/crawford-weimann"
                                class="footer-1-link-gray col-span-1 row-span-1">Team Member</a><a href="/company/blog"
                                class="footer-1-link-gray col-span-1 row-span-1">Blog</a><a
                                href="https://codebase-template.webflow.io/post/how-to-improve-web-design-process"
                                class="footer-1-link-gray col-span-1 row-span-1">Blog Post</a><a href="/company/careers"
                                class="footer-1-link-gray col-span-1 row-span-1">Careers</a><a
                                href="https://codebase-template.webflow.io/job/senior-product-engineer-backend"
                                class="footer-1-link-gray col-span-1 row-span-1">Careers Detail</a><a
                                href="/company/contact" class="footer-1-link-gray col-span-1 row-span-1">Contact</a><a
                                href="/company/legal" class="footer-1-link-gray col-span-1 row-span-1">Legal</a>
                        </div>

                        <div class="column-sm">
                            <div class="margin-bottom margin-3 col-span-1 row-span-1">
                                <h6 class="footer-1-nav-heading">Account</h6>
                            </div><a href="/account/sign-up" class="footer-1-link-gray col-span-1 row-span-1">Create
                                Account</a><a href="/account/sign-in"
                                class="footer-1-link-gray col-span-1 row-span-1">Sign In</a><a
                                href="/account/forgot-password" class="footer-1-link-gray col-span-1 row-span-1">Forgot
                                Password</a>
                        </div>
                    </div>
                </div>
            </div>
            <div class="footer-1-meta col-span-1 row-span-1">
                <div class="footer-row-base column-mobile">
                    <a href="#" class="footer-1-link-gray col-span-1 row-span-1">©
                        Template, Inc.</a>
                    <a href="/getting-started/style-guide" class="footer-1-link-gray col-span-1 row-span-1">Style
                        Guide</a><a href="/getting-started/instructions"
                        class="footer-1-link-gray col-span-1 row-span-1">Instructions</a><a
                        href="/getting-started/licensing"
                        class="footer-1-link-gray col-span-1 row-span-1">Licensing</a><a
                        href="/getting-started/changelog" class="footer-1-link-gray col-span-1 row-span-1">Changelog</a>
                </div>
            </div>
        </div>
    </div>
</template>



<style scoped>
.footer-grid {
    z-index: 5;
    grid-column-gap: 3em;
    grid-row-gap: 3em;
    grid-template-rows: auto;
    grid-template-columns: 1fr;
    grid-auto-columns: 1fr;
    justify-items: stretch;
    display: grid;
    position: relative;
}

.footer-1-cta-grid {
    grid-auto-columns: 1fr;
    display: grid;
    z-index: 1;
    width: 100%;
    max-width: 40em;
    grid-column-gap: 4em;
    grid-row-gap: 4em;
    grid-template-rows: auto;
    grid-template-columns: 1fr;
    align-items: center;
    justify-items: center;
    position: relative;
}

.cta-title-sm {
    letter-spacing: -.04em;
    font-size: 3em;
    font-weight: 700;
    line-height: 1.1;
}

.cta-row-base {
    gap: 1em;
    grid-template-rows: auto;
    grid-template-columns: auto;
    grid-auto-columns: auto;
    grid-auto-flow: column;
    justify-content: start;
    display: grid;
}

.button-animated {
    letter-spacing: -.03em;
    transition: color .2s cubic-bezier(.165, .84, .44, 1);
}

.button-hover-background {
    z-index: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, .1);
    border-radius: 9999px;
    position: absolute;
    top: 0%;
    bottom: 0%;
    left: 0%;
    right: 0%;
}

.footer-1-main-grid {
    display: grid;
    grid-auto-columns: 1fr;
    width: 100%;
    grid-column-gap: 4em;
    grid-row-gap: 4em;
    grid-template-rows: auto;
    grid-template-columns: auto 1fr;
}

.footer-1-sub-grid {
    display: grid;
    grid-auto-columns: 1fr;
    gap: 2em;
    grid-template-rows: auto;
    grid-template-columns: repeat(4, 1fr);
    align-items: start;
    margin-top: .5em;
}

.column-sm {
    grid-column-gap: .5em;
    grid-row-gap: .5em;
    grid-template-rows: auto;
    grid-template-columns: 1fr;
    grid-auto-columns: 1fr;
    justify-items: start;
    display: grid;
    position: relative;
}

.footer-1-nav-heading {
    color: var(--titles-links);
    letter-spacing: .01em;
    text-transform: uppercase;
    font-size: .625em;
    font-weight: 700;
}

h6 {
    margin-top: 0;
    margin-bottom: 0;
    line-height: 1.2;
}

.footer-1-link-gray {
    opacity: 1;
    color: var(--neutral-400);
    font-size: .875em;
    transition: opacity .25s, color .25s;
}

.footer-1-meta {
    border-top: 1px solid var(--border);
    padding-top: 1em;
}

.footer-row-base {
    grid-column-gap: 1em;
    grid-row-gap: 1em;
    grid-template-rows: auto;
    grid-template-columns: auto;
    grid-auto-columns: auto;
    grid-auto-flow: column;
    justify-content: start;
    display: grid;
}

@media (max-width: 479px) {
    .footer-grid {
        grid-column-gap: 3em;
        grid-row-gap: 1.5em;
    }

    .footer-1-cta-box {
        padding-left: 1.25em;
        padding-right: 1.25em;
    }

    .cta-title-sm {
        font-size: 1.75em;
    }

    .button-animated {
        font-size: 1em;
    }

    .footer-1-main-grid,
    .contact-list {
        grid-template-columns: 1fr;
    }

    .footer-1-sub-grid {
        grid-column-gap: 1em;
        grid-row-gap: 2em;
    }

    .footer-row-base.column-mobile {
        grid-auto-flow: row;
    }
}

a {
    color: var(--titles-links);
    text-decoration: none;
    transition: opacity .3s, background-color .3s, color .3s;
}

.image-contain {
    z-index: 5;
    width: 100%;
    object-fit: contain;
    line-height: 1;
    position: relative;
}

img {
    max-width: 100%;
    vertical-align: middle;
    display: inline-block;
}

@media (min-width: 500px) and (max-width: 767px) {
    .footer-1-cta-box {
        padding-left: 2em;
        padding-right: 2em;
    }

    .footer-1-cta-grid {
        grid-row-gap: 1em;
        text-align: center;
        grid-template-columns: 1fr;
        justify-items: center;
    }

    .cta-title-sm {
        font-size: 2.25em;
    }

    .footer-row-base.column-mobile {
        grid-auto-flow: row;
        gap: .75em;
    }
}

@media (min-width: 768px) and (max-width: 991px) {
    .footer-1-cta-grid {
        text-align: center;
        grid-template-columns: 1fr;
        justify-items: center;
    }

    .cta-title-sm {
        font-size: 2.5em;
    }

    .cta-button {
        justify-self: stretch;
    }

    .button-hover-background {
        display: none;
    }

    .footer-1-sub-grid {
        grid-template-columns: 1fr 1fr;
    }
}
</style>