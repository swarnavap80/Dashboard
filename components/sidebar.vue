<template>
  <div>
    <div class="sidebar dcreen w-52  shadow-md z-5 mt-[-46%]">
      <div class="logo flex gap-2">
        <img
          src="../public/images/instagram.png"
          alt=""
          class="h-8 mt-2 ml-4"
        />
        <h3 class="text-2xl mt-2 ml-2">iffe</h3>
      </div>
      <div class="menu h-84 w-24 mt-16 text-base">
        <h4 class="ml-4 text-violet-500">Menu</h4>
        <div class="icons mt-2 ml-6">
          <ul>
            <div class="icon-1 flex pt-4">
              <img src="../public/images/home.png" class="h-6" alt="" />
              <li class="p-1">Home</li>
            </div>
            <div class="icon-2 flex pt-4">
              <img src="../public/images/garage.png" class="h-6" alt="" />
              <li class="p-1">Garage</li>
            </div>
            <div class="icon-3 flex w-32 pt-4">
              <img src="../public/images/food.png" class="h-6" alt="" />
              <p>Service Menu</p>
            </div>

            <div class="icon-4 flex pt-4">
              <img src="../public/images/racer.png" class="h-6 mt-2" alt="" />
              <li class="p-1 mt-2">Racers</li>
            </div>
            <div class="icon-5 flex pt-4">
              <img src="../public/images/calculator.png" class="h-6" alt="" />
              <li class="p-1">Calculator</li>
            </div>
            <div class="icon-6 flex pt-4">
              <img src="../public/images/settings.png" class="h-6" alt="" />
              <li class="p-1">Settings</li>
            </div>
          </ul>
        </div>
      </div>
      <div class="scheduled_races h-32 w-24 mt-12 text-base">
        <h3 class="w-32 ml-4 text-violet-500">Scheduled races</h3>
        <div class="racer1 w-56 flex p-2 mt-4">
          <div
            class="b1 border-solid border-blue-400 w-6 border-2 rounded-full ml-2"
          ></div>
          <p class="ml-4">MotoGp 2022</p>
        </div>
        <div class="racer2 w-56 flex p-2">
          <div
            class="b1 border-solid border-red-400 w-6 border-2 rounded-full ml-2"
          ></div>
          <p class="ml-4">Dynamics 22</p>
        </div>
        <div class="racer3 w-56 flex p-2">
          <div
            class="b1 border-solid border-green-400 w-6 border-2 rounded-full ml-2"
          ></div>
          <p class="ml-4">Olympics</p>
        </div>
      </div>
      <div class="profile h-12 w-44 flex mt-12 ml-4 bg-[#F9FAFF]">
        <img src="../public/images/man.png" class="h-8 ml-2 mt-2" alt="" />
        <p class="p-2">Kilua</p>
        <img src="../public/images/upload.png" class="h-4 p-1 mt-3" alt="" />
      </div>
    </div>
  </div>
</template>

<script setup type="ts">

</script>
