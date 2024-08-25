<template>
  <div>
    <div class="nav shadow-md w-4.2/5 ml-52  h-24 flex overflow-x-hidden z-4">
      <div class="search1 w-5/12">
        <img
          src="../public/images/search-interface-symbol.png"
          class="h-4 absolute left-60 top-9"
          alt=""
        />
        <input
          type="search"
          placeholder="       search for race,cars or racers"
          class="search1 h-12 w-full border-2 rounded-lg ml-6 mt-4 border-gray-200"
        />
      </div>
      <div class="search2">
        <img
          src="../public/images/down-arrow.png"
          class="h-4 absolute left-[74%] top-9"
          alt=""
        />
        <input
          type="search"
          placeholder="       choose a car"
          class="search2 h-12 w-11/12 border-2 rounded-lg mt-4 ml-32 border-gray-200"
        />
      </div>
      <div class="images flex space-x-16 ml-44 mt-6">
        <img src="../public/images/notification.png" class="h-6" alt="" />
        <img src="../public/images/user.png" class="h-6" alt="" />
        <img src="../public/images/man.png" class="h-6" alt="" />
      </div>
    </div>
  </div>
</template>

<script setup type="ts"></script>
