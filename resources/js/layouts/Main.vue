<script setup>
import sidebar from '@/assets/sidebar.js';
import HeaderLayout from '@/layouts/HeaderLayout.vue';
import SidebarLayout from '@/layouts/SidebarLayout.vue';

import {onMounted} from 'vue';


onMounted(() => {
    window.HSStaticMethods.autoInit();
    sidebar();
});

</script>

<template>
<div class="main-wrapper">
    <HeaderLayout/>    
    <div class="body flex justify-start">
        <SidebarLayout/>  
        <div class="right w-full">
            <main >
                <div class="w-full min-h-[900px] bg-[#F1F4F6] p-[30px]">
                    <div id="bodyCard" class=" h-screen p-5 md:ml-[250px] rounded-md">
                        <slot></slot>
                    </div>
                </div>
            </main>
        </div>
    </div>
</div>
</template>

<style scoped>
.sidebar {
    transition: min-width 0.3s; /* Optional: Add a smooth transition effect */
  }

  #bodyCard {
    transition: margin-left 0.3s; /* Optional: Add a smooth transition effect */
  }
</style>