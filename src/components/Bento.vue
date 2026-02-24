<script setup lang="ts">
import { defineProps } from "vue";

const data = defineProps({
    firstname: {
        type: String,
        required: true,
    },
    secondname: {
        type: String,
        required: true,
    },
    value: {
        type: String,
        required: true,
    },
    color: {
        type: String,
        required: true,
    },
    imgSrc: {
        type: String,
        required: true,
    },
});
</script>

<template>
    <div
        class="rounded-xl grid grid-cols-1 sm:grid-cols-2 items-center justify-center gap-4"
        :style="{ backgroundColor: color }"
    >
        <img
            :src="imgSrc"
            alt="Bento Image"
            class="size-40 rounded-full object-cover object-top p-2"
        />

        <div class="text-center text-md-start">
            <div class="py-4">
                <p class="text-lg text-black">{{ firstname }}</p>
                <p class="text-lg text-black">{{ secondname }}</p>
            </div>
            <p class="text-2xl font-bold text-black text font-serif">
                {{ value }}
            </p>
        </div>
    </div>
</template>
