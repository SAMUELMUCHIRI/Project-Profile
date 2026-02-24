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
            <div
                @click="toogle"
                class="bg-[#CFA029] px-5 py-3 hover:bg-amber-400 rounded-t-xl"
            >
                <h3 class="text-white font-bold text-lg tracking-wide">
                    FOUNDATION MEMBERSHIP
                </h3>
            </div>
            <div class="bg-zinc-700 px-5 py-4 rounded-b-xl text-white">
                <p
                    :class="
                        isOpen
                            ? 'bg-zinc-700 text-sm leading-relaxed'
                            : 'hidden'
                    "
                >
                    We invest for you, in shares and in the Mansa-X global fund.
                    Service is free online with your personal representative,
                    but service in the office may have extra charges.
                </p>
            </div>
        </div>
    </div>
</template>
