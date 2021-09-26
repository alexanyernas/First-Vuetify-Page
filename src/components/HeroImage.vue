<template>
  <v-container class="pt-15">
      <v-row>
          <v-col lg="6">
              <h2 class="intro-text">Lorem ipsum dolor sit amet touya.</h2>
              <p class="description">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quibusdam sapiente pariatur eos eaque beatae tempore magni, nesciunt consectetur quis aut nam doloribus officia sunt voluptatem est distinctio, eum tenetur ut.</p>
              <v-btn class="white--text mr-10" color="primary" rounded>Get Started</v-btn>
              <v-btn class="white--text" color="indigo" rounded>
                  <v-icon>mdi-play-circle</v-icon> Watch Video
              </v-btn>
          </v-col>
          <v-col lg="6">
              <img width="100%" src="./../assets/2.png" alt="HeroImage">
          </v-col>
      </v-row>
  </v-container>
</template>

<script>
export default {
    name: 'HeroImage'
}
</script>

<style scoped>
.intro-text
{
    font-size: 60px;
    font-weight: bold;
    color: #444;
}

.description
{
    font-size: 19px;
    margin: 32px 0;
    color: #444444ba
}
</style>