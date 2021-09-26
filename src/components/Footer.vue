<template>
  <v-footer padless>
      <v-col lg="12">
          <v-row justify="center">
              <v-col lg="4" class="text-center">
                <v-toolbar-title class="brand">Alexanyer Naranjo</v-toolbar-title>
                <v-card-text>
                    <v-btn
                    v-for="icon in icons"
                    :key="icon"
                    class="mx-4 black--text"
                    icon
                    >
                    <v-icon size="24px">
                        {{ icon }}
                    </v-icon>
                    </v-btn>
                </v-card-text>
                <v-subheader>Lorem ipsum dolor sit amet consectetur adipisicing elit. Et corporis, quam accusantium eligendi voluptatum beatae, earum quo non error rerum quis. Magni doloremque quia voluptas ad! Architecto velit corporis repellendus!</v-subheader>
                <v-form class="mt-8">
                    <v-text-field label="Email" outlined dense/>
                    <v-btn color="blue" class="white--text" rounded>Subscribe Us</v-btn>
                </v-form>
              </v-col>
          </v-row>
          <v-col class="mt-10">
            <v-divider></v-divider>
            <v-subheader>
                Copyright Alexanyer Naranjo. All Rights Reserved 2021  {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
                <v-spacer></v-spacer>
                <strong>Designed by Alexanyer Naranjo</strong>
            </v-subheader>
          </v-col>
      </v-col>
    </v-card>
  </v-footer>
</template>

<script>
  export default {
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>