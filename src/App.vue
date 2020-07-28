<template>
  <div id="app">
    <main>
      <img src="./assets/logo.png" height="120" alt="Enyo Station" style="margin-bottom: 30px" />
      <div class>
        <embed src="https://s4.radio.co/s48426d56a/listen" width="300" height="200" />
      </div>
      <!-- <router-view></router-view> -->
    </main>
  </div>
</template>

<script>
import { Howl, Howler } from "howler";
export default {
  name: "app",
  data() {
    return {
      radioUrl: "https://s4.radio.co/s48426d56a/listen"
    };
  },
  methods: {
    // require("@/assets/animals_alligator_growl.mp3")
    // playSound() {
    //   var sound = new Howl({
    //     src: require("@/assets/animals_alligator_growl.mp3"),
    //     // src: "https://s4.radio.co/s48426d56a/listen",
    //     // autoplay: true,
    //     // loop: true,
    //     volume: 1,
    //     onplay: function() {
    //       console.log("Playing");
    //     }
    //     // onend: function() {
    //     //   console.log("Finished!");
    //     // }
    //   });
    //   // Play the sound.
    //   sound.play();
    // }
  },
  mounted: function() {
    // this.playSound();
    // var sound = new Howl({
    //   src: "https://s4.radio.co/s48426d56a/listen",
    //   autoplay: true,
    //   loop: true,
    //   volume: 0.5,
    //   onend: function() {
    //     console.log("Finished!");
    //   }
    // });
  }
};
</script>

<style>
body {
  margin: 0;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

main {
  text-align: center;
  margin-top: 40px;
}

header {
  margin: 0;
  height: 56px;
  padding: 0 16px 0 24px;
  background-color: #35495e;
  color: #ffffff;
}

header span {
  display: block;
  position: relative;
  font-size: 20px;
  line-height: 1;
  letter-spacing: 0.02em;
  font-weight: 400;
  box-sizing: border-box;
  padding-top: 16px;
}
</style>
