<template>
  <div class="flex">
    <div class="main h-screen w-52 shadow-md">
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
      <div class="profile h-12 w-44 flex mt-16 ml-4 bg-[#F9FAFF]">
        <img src="../public/images/man.png" class="h-8 ml-2 mt-2" alt="" />
        <p class="p-2">Kilua</p>
        <img src="../public/images/upload.png" class="h-4 p-1 mt-3" alt="" />
      </div>
    </div>
    <div class="side-main w-11/12 h-screen ">
      <div class="nav shadow-md w-full h-24 flex">
        <div class="search1 w-5/12">
          <img
            src="../public/images/search-interface-symbol.png"
            class="h-4 absolute left-60 top-9"
            alt=""
          />
          <input
            type="search"
            placeholder="       search for race,cars or racers"
            class="search1 h-12 w-full border-2 rounded-lg ml-8 mt-4 border-gray-200"
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
      <div class="box h-28 w-full flex space-x-28 mt-8">
        <div class="box1 h-20 w-20 ml-32 shadow-md w">
          <img
            src="../public/images/car-key.png"
            class="h-12 ml-4 mt-2"
            alt=""
          />
          <p class="text-center text-xs">Start</p>
        </div>
        <div class="box2 h-20 w-20 shadow-md w">
          <img
            src="../public/images/steering-wheel.png"
            class="h-12 ml-4 mt-2"
            alt=""
          />
          <p class="text-center text-xs">Drive</p>
        </div>
        <div class="box3 h-20 w-20 shadow-md w">
          <img
            src="../public/images/repair.png"
            class="h-12 ml-4 mt-2"
            alt=""
          />
          <p class="text-center text-xs">Maintainance</p>
        </div>
        <div class="box4 h-20 w-20 shadow-md w">
          <img
            src="../public/images/accumulator.png"
            class="h-12 ml-4 mt-2"
            alt=""
          />
          <p class="text-center text-xs">Battery</p>
        </div>
        <div class="box5 h-20 w-20 shadow-md w">
          <img src="../public/images/wheel.png" class="h-12 ml-4 mt-2" alt="" />
          <p class="text-center text-xs">Tires</p>
        </div>
        <div class="box6 h-20 w-20 shadow-md w">
          <img src="../public/images/lock.png" class="h-12 ml-4 mt-2" alt="" />
          <p class="text-center text-xs">Lock</p>
        </div>
      </div>
      <div class="car-container h-80 w-full flex">
        <h2 class="text-4xl mt-8 ml-24">Infiniti Renault</h2>
        <div class="trademark">
          <p class="mt-2">TM</p>
        </div>
        <img
          src="../public/images/formula1_car-removebg-preview.png"
          class="h-96 absolute left-64"
          alt=""
        />
        <div class="nav-key flex ml-72 mt-8 space-x-2">
          <div class="key1 shadow-md h-14 w-14">
            <img
              src="../public/images/left-chevron.png"
              class="h-6 ml-4 mt-4"
              alt=""
            />
          </div>
          <div class="key2 key1 shadow-md h-14 w-14">
            <img
              src="../public/images/right-arrow-angle.png"
              class="h-6 ml-4 mt-4"
              alt=""
            />
          </div>
        </div>
        <div class="details">
          <div class="det1 ml-32 mt-8 flex">
            <div class="img1">
              <img src="../public/images/trophy.png" class="h-6 mt-2" alt="" />
            </div>
            <div class="con1 ml-4">
              <h2 class="text-2xl">72</h2>
              <p>Champions</p>
            </div>
          </div>
          <div class="det2 ml-32 mt-4 flex">
            <div class="img2">
              <img src="../public/images/trophy.png" class="h-6 mt-2" alt="" />
            </div>
            <div class="con2 ml-4">
              <h2 class="text-2xl">32</h2>
              <p>skins</p>
            </div>
          </div>
          <div class="det3 ml-32 mt-4 flex">
            <div class="img3">
              <img src="../public/images/trophy.png" class="h-6 mt-2" alt="" />
            </div>
            <div class="con3 ml-4">
              <h2 class="text-2xl">64</h2>
              <p>Trophies won</p>
            </div>
          </div>
        </div>
      </div>
      <div class="graph h-32 w-full mt-10 space-x-52  flex">
              <div class="graph1 h-28 w-72  ml-52 shadow-md">
                  <img src="../public/images/Screenshot 2024-07-26 000940.png"  alt="">
              </div>
              <div class="graph2 h-28 w-72  shadow-md">
                   <img src="../public/images/Screenshot 2024-07-26 001001.png" alt="">
              </div>
</div>
    </div>
  
  </div>
</template>

<script setup></script>

