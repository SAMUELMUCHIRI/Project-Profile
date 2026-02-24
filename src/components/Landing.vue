<script setup>
import profile from "@/assets/images/profile.webp";
</script>
<template>
    <div class="h-full w-full px-5">
        <div
            class="rounded-xl flex items-center gap-6 justify-between border border-amber-600/50 bg-zinc-700/50 w-full p-4"
        >
            <!-- Profile Image -->
            <div class="flex-shrink-0">
                <img
                    :src="profile"
                    alt="Profile"
                    class="w-24 h-24 rounded-full object-cover object-top"
                />
            </div>

            <!-- Content -->
            <div class="flex flex-col gap-10">
                <p class="text-xl text-white font-medium">Michael</p>
                <p class="text-lg text-zinc-200 leading-relaxed">
                    You've officially joined<br />
                    your first investment<br />
                    knowledge club!
                </p>
            </div>
        </div>
    </div>
</template>
