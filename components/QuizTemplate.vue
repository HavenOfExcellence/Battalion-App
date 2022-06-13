<template>
  <div
    class="flex flex-col w-screen px-5 h-screen bg-[#1A1A1A] justify-center items-center"
  >
    <div class="flex flex-col items-start w-full">
      <h4 class="mt-10 text-xl text-white/60">Question 1 of 5</h4>
      <div class="mt-4 text-2xl text-white">
        What type of framework is Next.js?
      </div>
      <div
        class="flex items-center w-full py-4 pl-5 m-2 ml-0 space-x-2 border-2 cursor-pointer bg-white/5 border-white/10 rounded-xl"
      >
        <input type="radio" class="w-6 h-6 bg-black" />
        <p class="ml-6 text-white">ASDASD</p>
      </div>
      <div
        class="flex items-center w-full py-4 pl-5 m-2 ml-0 space-x-2 border-2 cursor-pointer bg-white/5 border-white/10 rounded-xl"
      >
        <input type="radio" class="w-6 h-6 bg-black" />
        <p class="ml-6 text-white">ASDASDasdasd</p>
      </div>
      <div className="flex justify-between w-full mt-4 text-white">
        <button className="w-[49%] py-3 bg-indigo-600 rounded-lg">
          Previous
        </button>
        <button className="w-[49%] py-3 bg-indigo-600 rounded-lg">Next</button>
      </div>
    </div>
  </div>
</template>
