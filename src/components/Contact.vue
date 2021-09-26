<template>
  <v-container class="my-15">
    <v-row justify="center">
        <v-col lg="12" class="text-center">
            <v-subheader class="text-h4 justify-center">Contact</v-subheader>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quisquam, at.</p>
        </v-col>
        <v-col lg="6">
          <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d125528.61711423936!2d-67.07680106780067!3d10.518829476265896!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8c2a58adcd824807%3A0x93dd2eae0a998483!2sCaracas%2C%20Distrito%20Capital!5e0!3m2!1ses-419!2sve!4v1632688232053!5m2!1ses-419!2sve" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
        </v-col>
        <v-col lg="6">
          <v-form ref="form">
            <v-text-field
              v-model="information.name"
              :counter="15"
              label="Name"
              required
            ></v-text-field>

            <v-text-field
              v-model="information.email"
              label="E-mail"
              required
            ></v-text-field>

            <v-textarea label="Massage" v-model="information.massage" no-resize></v-textarea>

            <v-btn color="indigo" class="mr-4 white--text">Send</v-btn>
          </v-form>
        </v-col>
    </v-row>
  </v-container> 
</template>

<script>
export default {
    name: 'Contact',
    data () {
      return {
        information: {
          name: '',
          email: '',
          massage: ''
        }
      }
    }
}
</script>