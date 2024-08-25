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
      "Welcome to Data Science On Maps Application .By accessing or using our Application, you agree to comply with and be bound by the following terms and conditions . Please read them carefully."
    ]
  },
  {
    title: "User Account",
    isOpen: false,
    points: [
      "Users may be required to create an account to access certain features of the Application.",
      "Users must provide accurate and up-to-date information when creating an account.",
      "Users are responsible for maintaining the confidentiality of their account credentials.",
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
    title: "Intellectual Property",
    isOpen: false,
    points: [
      "All content, including but not limited to text, graphics, code, and software, is the property of Data Science On Maps or its licensors.",
      
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
    title: "Privacy",
    isOpen: false,
    points: [
      "Data Science On Maps is committed to protecting the privacy of users. Please refer to our Privacy Policy for information on how we collect, use, and protect your personal information.",
    ]
  },
  {
    title: "Disclaimers",
    isOpen: false,
    points: [
      "The Application is provided on an as-in and as available basis. Data Science On Maps makes no warranties, expressed or implied, regarding the Application's accuracy, reliability, or availability.",
    ]
  },
   {
    title: "Termination",
    isOpen: false,
    points: [
     "Data Science On Maps reserves the right to suspend or terminate a user's access to the Application at any time and for any reason, without notice.",
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