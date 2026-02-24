<script setup lang="ts">
import Landing from "./components/Landing.vue";
import BentoGrid from "./components/BentoGrid.vue";
import Membership from "./components/Membership.vue";
import Membership1 from "./components/EconomyMembership.vue";
import SectionGreat from "./components/SectionGreat.vue";
import Footer from "./components/Footer.vue";
import CTA from "./components/CTA.vue";
</script>

<template>
    <main class="min-h-dvh bg-white">
        <div class="flex justify-center items-center">
            <div
                class="text-center gap-8 flex flex-col min-h-max justify-center bg-zinc-700 items-center py-8 rounded-b-xl container mx-auto"
            >
                <Landing />
                <BentoGrid />
            </div>
        </div>
        <div class="bg-inherit h-4"></div>

        <SectionGreat />
        <Membership />
        <Membership1 />
        <CTA />
        <Footer />
    </main>
</template>
