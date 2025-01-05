<script setup>
import { useForm } from "@inertiajs/vue3";

const form = useForm({
    email: "",
    password: "",
    remember: false,
});

const submit = () => {
    form.post(route("login"), {
        onFinish: () => form.reset("password"),
    });
};

</script>

<template>
    <div
        class="bg-surface-50 dark:bg-surface-900 flex items-center justify-center min-h-screen min-w-[100vw] overflow-hidden">
        <div class="flex flex-col items-center justify-center">
            <div>
                <div class="w-full bg-surface-0 dark:bg-surface-50 py-20 px-8 sm:px-20" style="border-radius: 7px">
                    <div class="text-center mb-8">
                        <div class="flex justify-center items-center">
                            <svg xmlns="http://www.w3.org/2000/svg" width="190" height="190" viewBox="0 0 4.233 4.233"
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
                        </div>
                        <div class="text-black text-3xl font-medium mb-4">PDL Order Management</div>
                        <span class="text-muted-color font-medium">Silahkan Login!</span>
                    </div>

                    <form @submit.prevent="submit">
                        <div>
                            <label for="email1"
                                class="block text-surface-900 dark:text-surface-0 text-xl font-medium mb-2">Email</label>
                            <InputText id="email1" type="text" placeholder="Email" class="w-full md:w-[30rem] mb-4"
                                v-model="form.email" />
                            <Message v-if="form.errors.email" class="mb-4" severity="error">{{ form.errors.email }}
                            </Message>

                            <label for="password1"
                                class="block text-surface-900 dark:text-surface-0 font-medium text-xl mb-2">Password</label>
                            <Password id="password1" v-model="form.password" placeholder="Password" :toggleMask="true"
                                class="mb-4" fluid :feedback="false"></Password>
                            <Message v-if="form.errors.password" class="mb-4" severity="error">{{ form.errors.password
                                }}</Message>

                            <div class="flex items-center justify-between mt-2 mb-8 gap-8">
                                <div class="flex items-center">
                                    <Checkbox v-model="form.remember" id="rememberme1" binary class="mr-2"></Checkbox>
                                    <label for="rememberme1">Remember me</label>
                                </div>
                                <span
                                    class="font-medium no-underline ml-2 text-right cursor-pointer text-primary">Forgot
                                    password?</span>
                            </div>
                            <Button type="submit" label="Sign In" class="w-full"></Button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.pi-eye {
    transform: scale(1.6);
    margin-right: 1rem;
}

.pi-eye-slash {
    transform: scale(1.6);
    margin-right: 1rem;
}
</style>
