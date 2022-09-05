<template>
  <v-app>
    <h1 class="mx-auto name">Hi, i'm JackPigPro!</h1>
    <h3 class="sub">YouTuber and Scratcher</h3>
    <v-row class="mx-4 mx-auto mt-3">
      <v-btn
        color="red"
        @click="redirect('https://bit.ly/jackpigpro')"
        class="mx-1 d"
        >YouTube</v-btn
      >
      <v-btn
        color="orange"
        class="mx-1 d"
        @click="redirect('https://scratch.mit.edu/users/JackPigPro/')"
        >Scratch</v-btn
      >
      <v-btn
        color="blue"
        class="mx-1 d"
        @click="redirect('https://www.buymeacoffee.com/JackPigPro')"
        >Donate</v-btn
      >
    </v-row>
    <v-divider></v-divider>
    <h1 class="mx-auto mt-3 mb-n6">Check out my Scratch games!</h1>
    <v-row class="mx-auto">
      <img
        src="https://cdn2.scratch.mit.edu/get_image/project/718554490_144x108.png"
        v-ripple
        @click="redirect('https://scratch.mit.edu/projects/718554490/')"
        class="im mx-1 ml-10"
      />
      <img
        src="https://uploads.scratch.mit.edu/get_image/project/615371178_144x108.png"
        v-ripple
        @click="redirect('https://scratch.mit.edu/projects/615371178/')"
        class="im mx-1"
      />
      <img
        src="https://uploads.scratch.mit.edu/get_image/project/629096505_144x108.png"
        v-ripple
        @click="redirect('https://scratch.mit.edu/projects/629096505/')"
        class="im mx-1"
      />
      <img
        src="https://cdn2.scratch.mit.edu/get_image/project/629475087_144x108.png"
        v-ripple
        @click="redirect('https://scratch.mit.edu/projects/629475087/')"
        class="im mx-1"
      />
      <img
        src="https://cdn2.scratch.mit.edu/get_image/project/632495662_144x108.png"
        v-ripple
        @click="redirect('https://scratch.mit.edu/projects/632495662/')"
        class="im mx-1 mr-10"
      />
    </v-row>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({}),
  methods: {
    redirect: function (url) {
      window.location.href = url;
    },
  },
};
</script>

<style scoped>
.name {
  font-size: 80px;
  font-weight: 500;
  color: #3f51b5;
  text-align: center;
  margin-top: 100px;
  /* make it a blueish gradient */
  background: -webkit-linear-gradient(#3f51b5, #2196f3);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: 1000;
}
.im {
  display: block;
  height: 216px;
  /* make it 108x144 */
  width: 288px;
  margin: 0 auto;
  margin-top: 50px;
  cursor: pointer;
  text-align: center;
  margin-left: auto;
  margin-right: auto;
  /* center the image */
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.sub {
  font-size: 30px;
  font-weight: 500;
  color: orange-red;
  text-align: center;
  /* make it a red/orangr gradient */
  font-weight: 600;
}
.pfp {
  width: 200px;
  height: 10px;
  border-radius: 10%;
  margin-top: 100px;
}

.d {
  /* make the font color white */
  color: white;
  font-weight: 600;
  text-align: center;
}
</style>
