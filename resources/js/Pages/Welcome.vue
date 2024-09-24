<script setup lang="ts">
import { Head, Link } from "@inertiajs/vue3";
import Header from "./components/HeaderComponent.vue";

defineProps<{
    canLogin?: boolean;
    canRegister?: boolean;
    laravelVersion: string;
    phpVersion: string;
}>();

</script>

<template>
    <Head title="Welcome" />
    <div class="bg-gray-50 dark:bg-zinc-800 dark:teal-400">
        <div class="relative min-h-screen">
            <div class="w-full">
                <main class="pt-2">
                    <div class="flex flex-col mx-36 space-y-4 h-screen">
                        <div class="grid grid-cols-12">
                            <Header />
                        </div>
                        <div
                            class="text-center border-2 dark:border-teal-600 bg-teal-200 py-2 dark:text-zinc-809 text-xl"
                        >
                            a customer message goes here!
                        </div>
                        <!-- <div
                            class="dark:bg-teal-200 py-2 grid grid-cols-12 pl-5 text-center"
                        >
                            <div>Home</div>
                            <div>Peripherals</div>
                            <div>Figures</div>
                            <div>Guides</div>
                            <div>Merchandise</div>
                            <div>About Us</div>
                        </div> -->
                        <div class="grid grid-cols-2 gap-4 py-2 w-full h-full text-center text-5xl font-VT323">
                            <div class="main-square dark:bg-blue-500 dark:border-blue-900 shadow-2xl shadow-blue-900">
                                Welcome to Retro World
                            </div>
                            <div class="main-square dark:bg-red-500 dark:border-red-900 shadow-2xl shadow-red-900">
                                We buy and sell retro games
                            </div>
                            <div class="main-square dark:bg-green-500 dark:border-green-900 shadow-2xl shadow-green-900">
                                Click here to Check out our selection of retro gaming and accessories!
                            </div>
                            <div class="main-square dark:bg-yellow-500 dark:border-yellow-900 shadow-2xl shadow-yellow-900">
                                Retro World is open Mon to Sat at 20 Osmaston Road, Derby, DE12HR
                            </div>
                            <Link href="" class="main-square col-span-2 dark:border-teal-600 bg-teal-200">
                                <div >Enter Our Shop!</div>
                            </Link>
                        </div>
                    </div>
                </main>
            </div>
        </div>
    </div>
</template>
