<template>
  <div id="home" class="bg-black text-white flex-1 ml-56">

      <div class="flex px-10">
        <div class="w-1/2 mr-4 flex mx-28 my-8">
          <div class="text-right">
            <img src="../assets/electron.png" alt="image" class="rounded-full w-40">
          </div>
        </div>
      </div>
      
      <!-- <button @click="playMusic()" class="text-right mx-60">
        <img src="../assets/play.svg" alt="image" class="flex items-center">
      </button> -->
      <div class="mx-32">
        <audio controls>
        <source src="../assets/demo.wav" type="audio/mpeg" class="bg-grey-darker">
      </audio>
      </div>
      
    <div class="absolute pin-b w-3/5 h-48">
      <div class="search-container text-center p-3 relative">
          <textarea style="resize: none" type="text" placeholder="Input some words" class="bg-grey-darkest text-grey-light text-xs h-40 w-full p-2 pl-5 border border-grey-dark rounded">
          </textarea>
      </div>
    </div>
    <div class="absolute pin-b pin-r w-28 p-5 h-36">
      <button class="text-white bg-grey-darker px-2 py-4 rounded-lg" @click="$router.go(-1)">CONVERT</button>
    </div>
  </div>
</template>

<script>

//var audio = new Audio('assets/better.mp3')
let audio = new Audio();
audio.src = "../assets/demo.wav";
audio.play()

export default {
  name: 'home',
  methods: {
    
  }
}
</script>


