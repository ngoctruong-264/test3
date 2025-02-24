<script setup>
import TelegramIcon from './TelegramIcon.vue'
import FacebookIcon from './FacebookIcon.vue'
import InstaIcon from './InstaIcon.vue'
import TwitterIcon from './TwitterIcon.vue'
import AppleIcon from './AppleIcon.vue'
import AndroidIcon from './AndroidIcon.vue'
import CustomAccordion from '../custom/CustomAccordion.vue'
</script>

<template>
  <div
    class="mh-[400px] bg-[#12294A] flex justify-between px-[20px] lg:px-[50px] xl:px-[120px] py-[30px] md:pt-[50px] text-[#90A2BD] leading-[21px] flex-col md:flex-row mt-[40px]"
  >
    <div class="md:hidden">
      <custom-accordion id="games" title="Games" :section="['Game 1', 'Game 2', 'Game 3']" />
      <custom-accordion
        id="about"
        title="About"
        :section="['Game 1', 'Game 2', 'Game 3']"
        class="mt-2"
      />
      <custom-accordion
        id="legal-information"
        title="Legal Information"
        :section="['Game 1', 'Game 2', 'Game 3']"
        class="mt-2"
      />
    </div>
    <span class="flex flex-col-reverse md:block">
      <div
        class="flex md:block px-[24px] py-[18px] md:p-0 bg-[#1A3157] md:bg-transparent rounded-[10px] justify-between mt-[20px] md:mt-0 items-center"
      >
        <div>
          <div class="font-medium text-2xl text-white">Help Center</div>
          <div class="text-[15px] mt-2">If you have any questions?</div>
        </div>
        <button
          class="text-white bg-[#3555FF] px-[10px] md:px-[54px] py-[9px] md:py-[12px] rounded-[10px] md:mt-4"
        >
          GET ANSWERS
        </button>
      </div>
      <div class="flex justify-between md:mt-[30px] mt-[20px] px-[20%] md:px-0">
        <telegram-icon />
        <facebook-icon />
        <insta-icon />
        <twitter-icon />
      </div>
      <div class="md:hidden text-center mt-[20px] text-white">Follow Us</div>
    </span>
    <span class="hidden md:block">
      <div class="text-white">Games</div>
      <div class="mt-4">Game 1</div>
      <div class="mt-4">Game 2</div>
      <div class="mt-4">Game 3</div>
      <div class="mt-4">Game 4</div>
    </span>
    <span class="hidden md:block">
      <div class="text-white">About</div>
      <div class="mt-4">About Us</div>
      <div class="mt-4">Promotions</div>
      <div class="mt-4">VIP</div>
      <div class="mt-4">Help Center</div>
      <div class="mt-4">Awards & Certificates</div>
      <div class="mt-4">App</div>
    </span>
    <span class="hidden md:block">
      <div class="text-white">Legal Information</div>
      <div class="mt-4">General Terms & Conditions</div>
      <div class="mt-4">Responsible Gaming Policy</div>
      <div class="mt-4">Sports Betting Rules</div>
      <div class="mt-4">Privacy and Cookies Policy</div>
      <div class="mt-4">Payment Methods</div>
      <div class="mt-4">Limits</div>
    </span>
    <span class="w-full md:w-[160px]">
      <div class="text-white bg-[#1A3157] px-[11px] rounded-[10px] hidden md:flex">
        <apple-icon class="min-w-[42px]" />
        Bluechip App for Mac OS
      </div>
      <div class="flex justify-between mt-3 gap-5 md:gap-0">
        <span
          class="w-1/2 md:w-[76px] flex flex-row md:flex-col items-center bg-[#1A3157] py-[6px] px-[11px] rounded-[10px]"
        >
          <android-icon />
          <span class="block md:hidden pl-2">
            <div class="text-white">Bluechip App</div>
            <div>for Android</div>
          </span>
          <span class="hidden md:block">Android</span>
        </span>
        <span
          class="w-1/2 md:w-[76px] flex flex-row md:flex-col items-center bg-[#1A3157] py-[6px] px-[11px] rounded-[10px]"
        >
          <apple-icon />

          <span class="block md:hidden pl-2">
            <div class="text-white">Bluechip App</div>
            <div>for iOS</div>
          </span>
          <span class="hidden md:block">IOS</span>
        </span>
      </div>
    </span>
  </div>
</template>
