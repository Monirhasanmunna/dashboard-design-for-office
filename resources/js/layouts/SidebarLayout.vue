<script setup>
import DashboardIcon from '@/components/Icons/DashboardIcon.vue';
import DotIcon from '@/components/Icons/DotIcon.vue';
import MenuArrowIcon from '@/components/Icons/MenuArrowIcon.vue';
</script>

<template>
    <div id="sidebar" class="sidebar w-[0px] sm:min-w-[250px]  bg-[#FFFFFF] dark:bg-gray-800 fixed h-full overflow-hidden overflow-y-auto">
        <nav class="hs-accordion-group py-6 px-[8px] w-full flex flex-col flex-wrap" data-hs-accordion-always-open>
            <ul class="space-y-2">
                <li>
                    <a  class="menu bg-[#EAFFF4] text-[#69AA8A]" href="#">
                        <DashboardIcon class="menu-icon" />
                        Dashboard
                    </a>
                </li>


                <li class="hs-accordion" id="account-accordion">
                    <button type="button" class="menu hs-accordion-toggle">
                        <svg class="flex-shrink-0 mt-0.5 size-4" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="18" cy="15" r="3"/><circle cx="9" cy="7" r="4"/><path d="M10 15H6a4 4 0 0 0-4 4v2"/><path d="m21.7 16.4-.9-.3"/><path d="m15.2 13.9-.9-.3"/><path d="m16.6 18.7.3-.9"/><path d="m19.1 12.2.3-.9"/><path d="m19.6 18.7-.4-1"/><path d="m16.8 12.3-.4-1"/><path d="m14.3 16.6 1-.4"/><path d="m20.7 13.8 1-.4"/></svg>
                        Account

                        <MenuArrowIcon />
                    </button>

                    <div id="account-accordion-child" class="hs-accordion-content sub-menu-content">
                        <ul class="p-2">
                            <li>
                            <a class="sub-menu" href="#">
                                <DotIcon class="sub-menu-icon" />
                                Link 1
                            </a>
                            </li>
                            <li>
                                <a class="sub-menu" href="#">
                                <DotIcon class="sub-menu-icon" />
                                Link 2
                            </a>
                            </li>
                            <li>
                                <a class="sub-menu" href="#">
                                <DotIcon class="sub-menu-icon" />
                                Link 3
                            </a>
                            </li>
                        </ul>
                    </div>
                </li>

            
            </ul>
        </nav>
    </div>
</template>

<style scoped>

</style>