<script setup>
import SecondaryButton from '@/Components/SecondaryButton.vue';

const smoothScroll = (id) => {
    document.body.click();
    document.querySelector(id).scrollIntoView({
        behavior: 'smooth'
    });
};
</script>

<template>
    <div class="bg-surface-0 light:bg-surface-900">
        <div id="home" class="landing-wrapper overflow-hidden">
            <div class="py-6 px-6 mx-0 md:mx-12 lg:mx-20 lg:px-20 flex items-center justify-between relative lg:static">
                <a class="flex items-center" href="#">
                    <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" viewBox="0 0 4.233 4.233" id="Code">
                        <g transform="translate(73.405 -1.965)" fill="#d85b53" class="color000000 svgShape">
                            <g fill="#d85b53" class="color000000 svgShape">
                                <g transform="translate(.046)" fill="#d85b53" class="color000000 svgShape">
                                    <g transform="translate(0 -.007)" fill="#d85b53" class="color000000 svgShape">
                                        <g transform="rotate(15 -70.276 3.716)" fill="#d85b53"
                                            class="color000000 svgShape">
                                            <g fill="#d85b53" class="color000000 svgShape">
                                                <g fill="#d85b53" class="color000000 svgShape">
                                                    <g transform="rotate(-15 -69.074 1.433)" fill="#d85b53"
                                                        class="color000000 svgShape">
                                                        <path fill="none" stroke="#26d7fe" stroke-linecap="round"
                                                            stroke-linejoin="round" stroke-width=".265"
                                                            d="M-72.156546 1.9792925v.6972338m.141005.7517733h-1.588978M-70.162882 3.4402534v1.4462578m-.396875.533983h-.988053M-71.347808 3.9767145h.389568c.146579 0 .264584.1180041.264584.2645833v.387501c0 .1465792-.118005.2645833-.264584.2645833h-.389568c-.146579 0-.264583-.1180041-.264583-.2645833v-.387501c0-.1465792.118004-.2645833.264583-.2645833zM-71.199503 4.4163529h.09715"
                                                            paint-order="markers fill stroke"
                                                            class="colorStroke000000 svgStroke"></path>
                                                        <rect width=".988" height=".988" x="-73.605" y="1.98"
                                                            fill="none" stroke="#26d7fe" stroke-linecap="round"
                                                            stroke-linejoin="round" stroke-width=".265"
                                                            paint-order="markers fill stroke" rx=".265" ry=".265"
                                                            class="colorStroke000000 svgStroke">
                                                        </rect>
                                                        <path fill="none" stroke="#26d7fe" stroke-linecap="round"
                                                            stroke-linejoin="round" stroke-width=".265"
                                                            d="M-73.174455 2.4621989h.09715M-71.611765 1.9792925v1.0521321c0 .2198687.177007.396875.396875.396875h.488573"
                                                            paint-order="markers fill stroke"
                                                            class="colorStroke000000 svgStroke"></path>
                                                        <rect width=".988" height=".988" x="70.164" y="1.98" fill="none"
                                                            stroke="#26d7fe" stroke-linecap="round"
                                                            stroke-linejoin="round" stroke-width=".265"
                                                            paint-order="markers fill stroke" rx=".265" ry=".265"
                                                            transform="scale(-1 1)" class="colorStroke000000 svgStroke">
                                                        </rect>
                                                        <path fill="none" stroke="#26d7fe" stroke-linecap="round"
                                                            stroke-linejoin="round" stroke-width=".265"
                                                            d="M-70.593856 2.4621989h-.09715M-72.156546 5.4204873v-.356336m0-.6957961c0-.2198687-.177007-.396875-.396875-.396875h-1.051098"
                                                            paint-order="markers fill stroke"
                                                            class="colorStroke000000 svgStroke"></path>
                                                        <rect width=".988" height=".988" x="-73.605" y="-5.42"
                                                            fill="none" stroke="#26d7fe" stroke-linecap="round"
                                                            stroke-linejoin="round" stroke-width=".265"
                                                            paint-order="markers fill stroke" rx=".265" ry=".265"
                                                            transform="scale(1 -1)" class="colorStroke000000 svgStroke">
                                                        </rect>
                                                        <path fill="none" stroke="#26d7fe" stroke-linecap="round"
                                                            stroke-linejoin="round" stroke-width=".265"
                                                            d="m -73.174455,4.9375809 h 0.09715"
                                                            paint-order="markers fill stroke"
                                                            class="colorStroke000000 svgStroke"></path>
                                                    </g>
                                                </g>
                                            </g>
                                        </g>
                                    </g>
                                </g>
                            </g>
                        </g>
                    </svg>
                    <span class="text-surface-900 light:text-surface-0 font-medium text-2xl leading-normal mr-20">

                    </span>
                </a>
                <Button class="lg:!hidden" text severity="secondary" rounded
                    v-styleclass="{ selector: '@next', enterFromClass: 'hidden', enterActiveClass: 'animate-scalein', leaveToClass: 'hidden', leaveActiveClass: 'animate-fadeout', hideOnOutsideClick: true }">
                    <i class="pi pi-bars !text-2xl"></i>
                </Button>
                <div
                    class="items-center bg-surface-0 light:bg-surface-900 grow justify-between hidden lg:flex absolute lg:static w-full left-0 top-full px-12 lg:px-0 z-20 rounded-border">
                    <ul
                        class="list-none p-0 m-0 flex lg:items-center select-none flex-col lg:flex-row cursor-pointer gap-8">
                        <li>
                            <a @click="smoothScroll('#hero')"
                                class="px-0 py-4 text-surface-900 light:text-surface-0 font-medium text-xl">
                                <span>Home</span>
                            </a>
                        </li>
                        <li>
                            <a @click="smoothScroll('#features')"
                                class="px-0 py-4 text-surface-900 light:text-surface-0 font-medium text-xl">
                                <span>Features</span>
                            </a>
                        </li>
                    </ul>
                    <div class="flex border-t lg:border-t-0 border-surface py-4 lg:py-0 mt-4 lg:mt-0 gap-2">
                        <Button label="Login" text as="router-link" to="/auth/login" rounded>
                        </Button>
                        <!-- <Button label="Register" to="/auth/login" rounded></Button> -->
                    </div>
                </div>
            </div>

            <div id="hero" class="flex flex-col pt-6 px-6 lg:px-20 overflow-hidden"
                style="background: linear-gradient(0deg, rgba(255, 255, 255, 0.2), rgba(255, 255, 255, 0.2)), radial-gradient(77.36% 256.97% at 77.36% 57.52%, rgb(238, 239, 175) 0%, rgb(195, 227, 250) 100%); clip-path: ellipse(150% 87% at 93% 13%)">
                <div class="mx-6 md:mx-20 mt-0 md:mt-6">
                    <h1 class="text-6xl font-bold text-gray-900 leading-tight"><span class="font-light block">Pemesanan
                        </span>PDL FTI UNISKA MAB</h1>
                    <p class="font-normal text-2xl leading-normal md:mt-4 text-gray-700">Fakultas Teknologi Informasi -
                        Universitas Islam Kalimantan Muhammad Arsyad Al Banjari Banjarmasin</p>
                    <!-- <Button label="Get Started" as="router-link" to="/" rounded class="!text-xl mt-8 !px-4"></Button> -->
                </div>
                <div class="flex justify-center md:justify-end">
                    <img src="/demo/images/landing/screen-1.png" alt="Hero Image" class="w-9/12 md:w-auto" />
                </div>
            </div>

            <div id="features" class="py-6 px-6 lg:px-20 mt-8 mx-0 lg:mx-20">
                <div class="grid grid-cols-12 gap-4 justify-center">
                    <div class="col-span-12 text-center mt-20 mb-6">
                        <div class="text-surface-900 light:text-surface-0 font-normal mb-2 text-4xl">Marvelous Features
                        </div>
                        <span class="text-muted-color text-2xl">Placerat in egestas erat...</span>
                    </div>

                    <div class="col-span-12 md:col-span-12 lg:col-span-4 p-0 lg:pr-8 lg:pb-8 mt-6 lg:mt-0">
                        <div
                            style="height: 160px; padding: 2px; border-radius: 10px; background: linear-gradient(90deg, rgba(253, 228, 165, 0.2), rgba(187, 199, 205, 0.2)), linear-gradient(180deg, rgba(253, 228, 165, 0.2), rgba(187, 199, 205, 0.2))">
                            <div class="p-4 bg-surface-0 light:bg-surface-900 h-full" style="border-radius: 8px">
                                <div class="flex items-center justify-center bg-yellow-200 mb-4"
                                    style="width: 3.5rem; height: 3.5rem; border-radius: 10px">
                                    <i class="pi pi-fw pi-users !text-2xl text-yellow-700"></i>
                                </div>
                                <h5 class="mb-2 text-surface-900 light:text-surface-0">Easy to Use</h5>
                                <span class="text-surface-600 light:text-surface-200">Posuere morbi leo urna
                                    molestie.</span>
                            </div>
                        </div>
                    </div>

                    <div class="col-span-12 md:col-span-12 lg:col-span-4 p-0 lg:pr-8 lg:pb-8 mt-6 lg:mt-0">
                        <div
                            style="height: 160px; padding: 2px; border-radius: 10px; background: linear-gradient(90deg, rgba(145, 226, 237, 0.2), rgba(251, 199, 145, 0.2)), linear-gradient(180deg, rgba(253, 228, 165, 0.2), rgba(172, 180, 223, 0.2))">
                            <div class="p-4 bg-surface-0 light:bg-surface-900 h-full" style="border-radius: 8px">
                                <div class="flex items-center justify-center bg-cyan-200 mb-4"
                                    style="width: 3.5rem; height: 3.5rem; border-radius: 10px">
                                    <i class="pi pi-fw pi-palette !text-2xl text-cyan-700"></i>
                                </div>
                                <h5 class="mb-2 text-surface-900 light:text-surface-0">Fresh Design</h5>
                                <span class="text-surface-600 light:text-surface-200">Semper risus in hendrerit.</span>
                            </div>
                        </div>
                    </div>

                    <div class="col-span-12 md:col-span-12 lg:col-span-4 p-0 lg:pb-8 mt-6 lg:mt-0">
                        <div
                            style="height: 160px; padding: 2px; border-radius: 10px; background: linear-gradient(90deg, rgba(145, 226, 237, 0.2), rgba(172, 180, 223, 0.2)), linear-gradient(180deg, rgba(172, 180, 223, 0.2), rgba(246, 158, 188, 0.2))">
                            <div class="p-4 bg-surface-0 light:bg-surface-900 h-full" style="border-radius: 8px">
                                <div class="flex items-center justify-center bg-indigo-200"
                                    style="width: 3.5rem; height: 3.5rem; border-radius: 10px">
                                    <i class="pi pi-fw pi-map !text-2xl text-indigo-700"></i>
                                </div>
                                <div class="mt-6 mb-1 text-surface-900 light:text-surface-0 text-xl font-semibold">Well
                                    Documented</div>
                                <span class="text-surface-600 light:text-surface-200">Non arcu risus quis varius quam
                                    quisque.</span>
                            </div>
                        </div>
                    </div>

                    <div class="col-span-12 md:col-span-12 lg:col-span-4 p-0 lg:pr-8 lg:pb-8 mt-6 lg:mt-0">
                        <div
                            style="height: 160px; padding: 2px; border-radius: 10px; background: linear-gradient(90deg, rgba(187, 199, 205, 0.2), rgba(251, 199, 145, 0.2)), linear-gradient(180deg, rgba(253, 228, 165, 0.2), rgba(145, 210, 204, 0.2))">
                            <div class="p-4 bg-surface-0 light:bg-surface-900 h-full" style="border-radius: 8px">
                                <div class="flex items-center justify-center bg-slate-200 mb-4"
                                    style="width: 3.5rem; height: 3.5rem; border-radius: 10px">
                                    <i class="pi pi-fw pi-id-card !text-2xl text-slate-700"></i>
                                </div>
                                <div class="mt-6 mb-1 text-surface-900 light:text-surface-0 text-xl font-semibold">
                                    Responsive Layout</div>
                                <span class="text-surface-600 light:text-surface-200">Nulla malesuada pellentesque
                                    elit.</span>
                            </div>
                        </div>
                    </div>

                    <div class="col-span-12 md:col-span-12 lg:col-span-4 p-0 lg:pr-8 lg:pb-8 mt-6 lg:mt-0">
                        <div
                            style="height: 160px; padding: 2px; border-radius: 10px; background: linear-gradient(90deg, rgba(187, 199, 205, 0.2), rgba(246, 158, 188, 0.2)), linear-gradient(180deg, rgba(145, 226, 237, 0.2), rgba(160, 210, 250, 0.2))">
                            <div class="p-4 bg-surface-0 light:bg-surface-900 h-full" style="border-radius: 8px">
                                <div class="flex items-center justify-center bg-orange-200 mb-4"
                                    style="width: 3.5rem; height: 3.5rem; border-radius: 10px">
                                    <i class="pi pi-fw pi-star !text-2xl text-orange-700"></i>
                                </div>
                                <div class="mt-6 mb-1 text-surface-900 light:text-surface-0 text-xl font-semibold">Clean
                                    Code</div>
                                <span class="text-surface-600 light:text-surface-200">Condimentum lacinia quis vel
                                    eros.</span>
                            </div>
                        </div>
                    </div>

                    <div class="col-span-12 md:col-span-12 lg:col-span-4 p-0 lg:pb-8 mt-6 lg:mt-0">
                        <div
                            style="height: 160px; padding: 2px; border-radius: 10px; background: linear-gradient(90deg, rgba(251, 199, 145, 0.2), rgba(246, 158, 188, 0.2)), linear-gradient(180deg, rgba(172, 180, 223, 0.2), rgba(212, 162, 221, 0.2))">
                            <div class="p-4 bg-surface-0 light:bg-surface-900 h-full" style="border-radius: 8px">
                                <div class="flex items-center justify-center bg-pink-200 mb-4"
                                    style="width: 3.5rem; height: 3.5rem; border-radius: 10px">
                                    <i class="pi pi-fw pi-moon !text-2xl text-pink-700"></i>
                                </div>
                                <div class="mt-6 mb-1 text-surface-900 light:text-surface-0 text-xl font-semibold">light
                                    Mode</div>
                                <span class="text-surface-600 light:text-surface-200">Convallis tellus id interdum velit
                                    laoreet.</span>
                            </div>
                        </div>
                    </div>

                    <div class="col-span-12 md:col-span-12 lg:col-span-4 p-0 lg:pr-8 mt-6 lg:mt-0">
                        <div
                            style="height: 160px; padding: 2px; border-radius: 10px; background: linear-gradient(90deg, rgba(145, 210, 204, 0.2), rgba(160, 210, 250, 0.2)), linear-gradient(180deg, rgba(187, 199, 205, 0.2), rgba(145, 210, 204, 0.2))">
                            <div class="p-4 bg-surface-0 light:bg-surface-900 h-full" style="border-radius: 8px">
                                <div class="flex items-center justify-center bg-teal-200 mb-4"
                                    style="width: 3.5rem; height: 3.5rem; border-radius: 10px">
                                    <i class="pi pi-fw pi-shopping-cart !text-2xl text-teal-700"></i>
                                </div>
                                <div class="mt-6 mb-1 text-surface-900 light:text-surface-0 text-xl font-semibold">Ready
                                    to Use</div>
                                <span class="text-surface-600 light:text-surface-200">Mauris sit amet massa
                                    vitae.</span>
                            </div>
                        </div>
                    </div>

                    <div class="col-span-12 md:col-span-12 lg:col-span-4 p-0 lg:pr-8 mt-6 lg:mt-0">
                        <div
                            style="height: 160px; padding: 2px; border-radius: 10px; background: linear-gradient(90deg, rgba(145, 210, 204, 0.2), rgba(212, 162, 221, 0.2)), linear-gradient(180deg, rgba(251, 199, 145, 0.2), rgba(160, 210, 250, 0.2))">
                            <div class="p-4 bg-surface-0 light:bg-surface-900 h-full" style="border-radius: 8px">
                                <div class="flex items-center justify-center bg-blue-200 mb-4"
                                    style="width: 3.5rem; height: 3.5rem; border-radius: 10px">
                                    <i class="pi pi-fw pi-globe !text-2xl text-blue-700"></i>
                                </div>
                                <div class="mt-6 mb-1 text-surface-900 light:text-surface-0 text-xl font-semibold">
                                    Modern
                                    Practices</div>
                                <span class="text-surface-600 light:text-surface-200">Elementum nibh tellus molestie
                                    nunc
                                    non.</span>
                            </div>
                        </div>
                    </div>

                    <div class="col-span-12 md:col-span-12 lg:col-span-4 p-0 lg-4 mt-6 lg:mt-0">
                        <div
                            style="height: 160px; padding: 2px; border-radius: 10px; background: linear-gradient(90deg, rgba(160, 210, 250, 0.2), rgba(212, 162, 221, 0.2)), linear-gradient(180deg, rgba(246, 158, 188, 0.2), rgba(212, 162, 221, 0.2))">
                            <div class="p-4 bg-surface-0 light:bg-surface-900 h-full" style="border-radius: 8px">
                                <div class="flex items-center justify-center bg-purple-200 mb-4"
                                    style="width: 3.5rem; height: 3.5rem; border-radius: 10px">
                                    <i class="pi pi-fw pi-eye !text-2xl text-purple-700"></i>
                                </div>
                                <div class="mt-6 mb-1 text-surface-900 light:text-surface-0 text-xl font-semibold">
                                    Privacy</div>
                                <span class="text-surface-600 light:text-surface-200">Neque egestas congue
                                    quisque.</span>
                            </div>
                        </div>
                    </div>

                    <div class="col-span-12 mt-20 mb-20 p-2 md:p-20"
                        style="border-radius: 20px; background: linear-gradient(0deg, rgba(255, 255, 255, 0.6), rgba(255, 255, 255, 0.6)), radial-gradient(77.36% 256.97% at 77.36% 57.52%, #efe1af 0%, #c3dcfa 100%)">
                        <div class="flex flex-col justify-center items-center text-center px-4 py-4 md:py-0">
                            <div class="text-gray-900 mb-2 text-3xl font-semibold">Joséphine Miller</div>
                            <span class="text-gray-600 text-2xl">Peak Interactive</span>
                            <p class="text-gray-900 sm:line-height-2 md:line-height-4 text-2xl mt-6"
                                style="max-width: 800px">
                                “Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat
                                nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
                                officia deserunt mollit anim id est laborum.”
                            </p>
                            <img src="/demo/images/landing/peak-logo.svg" class="mt-6" alt="Company logo" />
                        </div>
                    </div>
                </div>
            </div>

            <div class="py-6 px-6 mx-0 mt-20 lg:mx-20">
                <div class="grid grid-cols-12 gap-4">
                    <div class="col-span-12 md:col-span-2">
                        <a @click="smoothScroll('#home')"
                            class="flex flex-wrap items-center justify-center md:justify-start md:mb-0 mb-4 cursor-pointer">
                            <svg xmlns="http://www.w3.org/2000/svg" width="130" height="130" viewBox="0 0 4.233 4.233"
                                id="Code">
                                <g transform="translate(73.405 -1.965)" fill="#d85b53" class="color000000 svgShape">
                                    <g fill="#d85b53" class="color000000 svgShape">
                                        <g transform="translate(.046)" fill="#d85b53" class="color000000 svgShape">
                                            <g transform="translate(0 -.007)" fill="#d85b53"
                                                class="color000000 svgShape">
                                                <g transform="rotate(15 -70.276 3.716)" fill="#d85b53"
                                                    class="color000000 svgShape">
                                                    <g fill="#d85b53" class="color000000 svgShape">
                                                        <g fill="#d85b53" class="color000000 svgShape">
                                                            <g transform="rotate(-15 -69.074 1.433)" fill="#d85b53"
                                                                class="color000000 svgShape">
                                                                <path fill="none" stroke="#26d7fe"
                                                                    stroke-linecap="round" stroke-linejoin="round"
                                                                    stroke-width=".265"
                                                                    d="M-72.156546 1.9792925v.6972338m.141005.7517733h-1.588978M-70.162882 3.4402534v1.4462578m-.396875.533983h-.988053M-71.347808 3.9767145h.389568c.146579 0 .264584.1180041.264584.2645833v.387501c0 .1465792-.118005.2645833-.264584.2645833h-.389568c-.146579 0-.264583-.1180041-.264583-.2645833v-.387501c0-.1465792.118004-.2645833.264583-.2645833zM-71.199503 4.4163529h.09715"
                                                                    paint-order="markers fill stroke"
                                                                    class="colorStroke000000 svgStroke"></path>
                                                                <rect width=".988" height=".988" x="-73.605" y="1.98"
                                                                    fill="none" stroke="#26d7fe" stroke-linecap="round"
                                                                    stroke-linejoin="round" stroke-width=".265"
                                                                    paint-order="markers fill stroke" rx=".265"
                                                                    ry=".265" class="colorStroke000000 svgStroke">
                                                                </rect>
                                                                <path fill="none" stroke="#26d7fe"
                                                                    stroke-linecap="round" stroke-linejoin="round"
                                                                    stroke-width=".265"
                                                                    d="M-73.174455 2.4621989h.09715M-71.611765 1.9792925v1.0521321c0 .2198687.177007.396875.396875.396875h.488573"
                                                                    paint-order="markers fill stroke"
                                                                    class="colorStroke000000 svgStroke"></path>
                                                                <rect width=".988" height=".988" x="70.164" y="1.98"
                                                                    fill="none" stroke="#26d7fe" stroke-linecap="round"
                                                                    stroke-linejoin="round" stroke-width=".265"
                                                                    paint-order="markers fill stroke" rx=".265"
                                                                    ry=".265" transform="scale(-1 1)"
                                                                    class="colorStroke000000 svgStroke"></rect>
                                                                <path fill="none" stroke="#26d7fe"
                                                                    stroke-linecap="round" stroke-linejoin="round"
                                                                    stroke-width=".265"
                                                                    d="M-70.593856 2.4621989h-.09715M-72.156546 5.4204873v-.356336m0-.6957961c0-.2198687-.177007-.396875-.396875-.396875h-1.051098"
                                                                    paint-order="markers fill stroke"
                                                                    class="colorStroke000000 svgStroke"></path>
                                                                <rect width=".988" height=".988" x="-73.605" y="-5.42"
                                                                    fill="none" stroke="#26d7fe" stroke-linecap="round"
                                                                    stroke-linejoin="round" stroke-width=".265"
                                                                    paint-order="markers fill stroke" rx=".265"
                                                                    ry=".265" transform="scale(1 -1)"
                                                                    class="colorStroke000000 svgStroke"></rect>
                                                                <path fill="none" stroke="#26d7fe"
                                                                    stroke-linecap="round" stroke-linejoin="round"
                                                                    stroke-width=".265"
                                                                    d="m -73.174455,4.9375809 h 0.09715"
                                                                    paint-order="markers fill stroke"
                                                                    class="colorStroke000000 svgStroke"></path>
                                                            </g>
                                                        </g>
                                                    </g>
                                                </g>
                                            </g>
                                        </g>
                                    </g>
                                </g>
                            </svg>
                            <!-- <h4 class="font-medium text-3xl text-surface-900 light:text-surface-0">SAKAI</h4> -->
                        </a>
                    </div>

                    <div class="col-span-12 md:col-span-10">
                        <div class="grid grid-cols-12 gap-8 text-center md:text-left">
                            <div class="col-span-12 md:col-span-3">
                                <h4
                                    class="font-medium text-2xl leading-normal mb-4 text-surface-900 light:text-surface-0">
                                    Fakultas Teknologi Informasi </h4>
                                <a
                                    class="leading-normal text-xl block cursor-pointer mb-2 text-surface-700 light:text-surface-100">BEM
                                    FTI</a>
                            </div>
                            <div class="col-span-12 md:col-span-3">
                                <h4
                                    class="font-medium text-2xl leading-normal mb-4 text-surface-900 light:text-surface-0">
                                    Alamat</h4>
                                <p class="leading-normal text-xl block  mb-2 text-surface-700 light:text-surface-100">
                                    No.,
                                    Jl. Cemara Raya No.58, Sungai Miai, Kec. Banjarmasin Utara, Kota Banjarmasin,
                                    Kalimantan Selatan 70123</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
