<template>
  <div class="position-static card d-flex justify-center align-center myBorder">
    <div class="d-flex flex-column justify-center align-center content">
      <h1 class="card-title">A PROPOS DE MOI</h1>
      <p class="text-subtitle-1">Cliquer ou scroller pour en apprendre plus sur moi</p>
      <button @click="scrolling()" class="readMore"><v-icon>mdi-arrow-down</v-icon>En lire +</button>
    </div>
  </div>

  <div class="spacer"></div>

  <div id="test" class="card d-flex justify-center align-center opacity-0" v-scroll="handleScroll">
    <div class="d-flex flex-column justify-center align-center">
      <div class="d-flex flex-row align-center">
        <v-avatar image="../../public/profile_picture.jpg" size="53"></v-avatar>
        <h1 class="card-title mx-4">PARPAILLON Olivier</h1>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CompAboutMe",
  data() {
    return {
      scroller: 0,
    }
  },
  methods: {
    handleScroll() {
      const scroller = window.scrollY;
      const divToShow = document.getElementById("test");
      console.log(scroller);
      if (scroller > 365) {
        divToShow.classList.replace('opacity-0', 'opacity-100');
      }
    },

    scrolling() {
      this.scroller += 10
    }
  },
}
</script>