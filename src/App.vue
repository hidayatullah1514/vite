<template>
 <div class="container mx-auto px-4 flex flex-col md:flex-row items-start">
    <HelloWorld msg="22FTT1514" class="text-center md:text-left" />
    <h1 class="read-the-docs text-xl md:text-2xl lg:text-3xl">
      Hi, My Name Is Muhammad Hidayatullah Bin Abas
    </h1>
    <p class="text-sm md:text-base">
      A student from DWDT08 who have a lot of datelines waiting for him
    </p>
     </div>
     <div class="container mx-auto px-4 flex flex-col md:flex-row items-start">
    <img
      :src="exampleImage"
      alt="Example Image"
      class="w-full md:w-1/2 lg:w-1/3 self-center"
    />
    <img
      :src="exampleImage1"
      alt="Example Image1"
      class="w-full md:w-1/2 lg:w-1/3 mt-4 md:mt-0 self-center"
    />
    </div>
   <div class="container mx-auto px-4 flex flex-col md:flex-row items-start">
      <img
      :src="exampleImage2"
      alt="Example Image2"
      class="w-full md:w-1/2 lg:w-1/3 mt-4 md:mt-0 self-center"
    />
    </div>

</template>

<script setup lang="ts">
import HelloWorld from "./components/HelloWorld.vue";
import exampleImage from "./assets/passportphoto.jpg";
import exampleImage1 from "./assets/passportphoto1.jpg";
import exampleImage2 from "./assets/passportphoto2.jpeg";
</script>

<style scoped>
.container {
 display: flex;
 flex-direction: column;
 align-items: flex-start; /* Align items to the start (top) */
}
@media (min-width: 640px) {
 .container {
    flex-direction: row;
 }
}
@media (min-width: 1024px) {
 .container {
    flex-direction: row;
 }
}

.responsive-image {
 max-width: 100%;
 height: auto;
}

h1 {
 font-size: clamp(1.5rem, 4vw, 3rem);
}

p {
 font-size: clamp(1rem, 2vw, 1.5rem);
}

/* Add this to center the images vertically */
img {
 align-self: center;
 width: 50%; /* Make the image responsive */
 height: 50%; /* Set the height to 100% to match the width */
 object-fit: cover;
}
</style>
