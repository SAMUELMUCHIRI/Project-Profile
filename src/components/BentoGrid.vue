<script setup lang="ts">
import Bento from "./Bento.vue";
import man1 from "@/assets/images/man1.webp";
import man2 from "@/assets/images/man2.webp";
import woman1 from "@/assets/images/woman1.webp";
import woman2 from "@/assets/images/woman2.webp";
</script>

<template>
    <div class="h-full w-full px-5">
        <div class="grid grid-cols-2 gap-4 w-full h-full flex-1">
            <Bento
                :imgSrc="man1"
                firstname="Bernard"
                secondname="Makodingo"
                value="350"
                color="#f7d3d4"
            />
            <Bento
                :imgSrc="man2"
                firstname="kigSmall"
                secondname="Foot"
                value="225"
                color="#d8e8aa"
            />
            <Bento
                :imgSrc="woman1"
                firstname="Caroline"
                secondname="Likhoi"
                value="117"
                color="#efd8b1"
            />
            <Bento
                :imgSrc="woman2"
                firstname="Caroline"
                secondname="Likhoi"
                value="321"
                color="#f7d3d4"
            />
        </div>
    </div>
</template>
