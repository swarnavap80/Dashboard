<template>
  <div>
    <h1 class="text-center text-3xl mt-4">Terms And Conditions Data Science on Maps</h1>
    <div v-for="(accordion, index) in accordions" :key="index" class="mb-4 mt-4">
      <div
        class="accordion1 h-12 w-2/3  ml-[15%] bg-[#FFD35A] rounded-md cursor-pointer relative flex items-center px-4"
        @click="toggleAccordion(index)"
      >
        <span> {{ accordion.title }} </span>
        <img
          :class="{'rotate-180': accordion.isOpen}"
          src="/images/down-arrow.png"
          class="h-8 w-8 cursor-pointer absolute right-4 transition-transform duration-300"
          alt="Toggle accordion"
        >
      </div>
      <transition
        name="accordion"
        enter-active-class="transition duration-300 ease-out"
        leave-active-class="transition duration-300 ease-in"
        enter-from-class="transform scale-y-0 opacity-0"
        enter-to-class="transform scale-y-100 opacity-100"
        leave-from-class="transform scale-y-100 opacity-100"
        leave-to-class="transform scale-y-0 opacity-0"
      >
        <div v-if="accordion.isOpen" class="accordion-content p-4 bg-white border border-[#FFDA76] w-2/3 ml-[15%] rounded-md origin-top">
          <ul class="list-disc pl-5 space-y-2">
            <li v-for="(point, pointIndex) in accordion.points" :key="pointIndex">
              {{ point }}
            </li>
              
          </ul>
        </div>
      </transition>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const accordions = ref([
  {
    title: "Introduction",
    isOpen: false,
    points: [
      "Welcome to Data Science on Maps. We value your privacy and are committed to protecting your personal information. This Privacy and Policy document outlines how we collect, use, and safeguard your data when you use our application."
    ]
  },
  {
    title: " Information We Collect",
    isOpen: false,
    points: [
      "Personal Information: When you create an account or interact with our application, we may collect personal details such as your name, email address, and any other information you voluntarily provide.",
      "Usage Data: We collect data on how you use the application, including the features you interact with, the types of visualizations you create, and your coding activities.",
      "Technical Data: Information about your device, such as IP address, browser type, operating system, and usage patterns, may be collected to improve your experience and maintain the security of our services.",
    ]
  },
  {
    title: "Use of the Application",
    isOpen: false,
    points: [
      "The Application is intended for educational and informational purposes only",
      "Users may not use the Application for any illegal or unauthorized purpose.",
    ]
  },
  {
    title: "How We Use Your Information",
    isOpen: false,
    points: [
      "Usage Data: We collect data on how you use the application, including the features you interact with, the types of visualizations you create, and your coding activities.",
      "Technical Data: Information about your device, such as IP address, browser type, operating system, and usage patterns, may be collected to improve your experience and maintain the security of our services.",
      
    ]
  },
  {
    title: "User Generated Content",
    isOpen: false,
    points: [
     "Users may have the opportunity to create and share content on the Application, such as visualizations or code.",
     "By submitting content, users grant [Your Company Name] a worldwide, royalty-free, and non-exclusive license to use, reproduce, modify, and distribute the content in connection with the Application.",
    ]
  },
  {
    title: "Sharing Your Informations",
    isOpen: false,
    points: [
      "Legal Requirements: We may disclose your information if required by law or in response to valid legal requests from governmental authorities.",
    ]
  },
  {
    title: "Data Security",
    isOpen: false,
    points: [
      "We implement industry-standard security measures to protect your data from unauthorized access, disclosure, or misuse. However, please note that no method of data transmission or storage is entirely secure.",
    ]
  },
   {
    title: "User Rights",
    isOpen: false,
    points: [
     "Data Deletion: You may request the deletion of your account and associated data. Please be aware that certain information may need to be retained for legal or operational reasons.",
    ]
  },
  {
    title: "Cookies and Tracking Technologies",
    isOpen: false,
    points: [
     "We may use cookies and similar tracking technologies to enhance your experience, analyze usage patterns, and improve our services. You can control cookie settings through your browser preferences.",
    ]
  },
])

const toggleAccordion = (index: number) => {
  accordions.value[index].isOpen = !accordions.value[index].isOpen
}


</script>

<style scoped>
.accordion-content {
  overflow: hidden;
}
</style>