<template>
  <v-container class="my-15">
      <v-row justify="center">
          <v-col lg="12" class="text-center">
              <v-subheader class="text-h4 justify-center">Projects</v-subheader>
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vel, doloremque.</p>
          </v-col>
          <v-col lg="4" v-for="project in 3" :key="project">
              <v-card max-width="374" class="mx-auto my-12">
                <v-img height="250" src="./../assets/app.jpg"></v-img>
                <v-card-title>Project</v-card-title>
                <v-card-text>
                    <div>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Voluptatum, pariatur!</div>
                </v-card-text>
                <v-divider class="mx-4"></v-divider>
                <v-card-actions>
                    <v-btn color="indigo" rounded class="white--text py-5">View Details</v-btn>
                    <v-spacer />
                    <v-rating
                        :value="4.5"
                        color="amber"
                        dense
                        half-increments
                        readonly
                        size="14"
                    ></v-rating>
                </v-card-actions>
              </v-card>
          </v-col>
      </v-row>
  </v-container>
</template>

<script>
export default {
    name: 'Project'
}
</script>