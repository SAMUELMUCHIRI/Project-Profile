<script setup lang="ts">
import { ref } from "vue";

const isOpen = ref(true);
function toogle() {
    isOpen.value = !isOpen.value;
    console.log(isOpen.value);
}
</script>

<template>
    <div class="flex min-h-max justify-center items-center py-2">
        <div class="w-full h-full flex-1 flex flex-col container mx-auto p-2">
            <div @click="toogle" class="bg-slate-500 px-5 py-3 rounded-t-xl">
                <h3 class="text-white font-bold text-lg tracking-wide">
                    ECONOMY MEMBERSHIP
                </h3>
            </div>
            <div class="bg-zinc-700 text-white px-5 py-4 rounded-b-xl">
                <p
                    :class="
                        isOpen
                            ? 'bg-zinc-700 text-sm leading-relaxed'
                            : 'hidden'
                    "
                >
                    We will invest your money for you at a guaranteed rate with
                    the Mansa-X global fund. Service is free online with your
                    personal representative, but service in the office may have
                    extra charges.
                </p>
            </div>
        </div>
    </div>
</template>
