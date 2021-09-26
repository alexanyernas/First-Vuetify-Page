<template>
  <v-container class="my-5">
      <v-row justify="center">
          <v-col lg="12" class="text-center">
              <v-subheader class="text-h4 justify-center">Portfolio</v-subheader>
              <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vel, doloremque.</p>
          </v-col>
          <v-col lg="12">
              <div class="text-center">
                    <v-chip @click="activePortfolio = 'webapp'" :color="activePortfolio === 'webapp' ? 'indigo white--text' : ''" class="mx-5">
                        Web App
                    </v-chip>
                    <v-chip @click="activePortfolio = 'mobileapp'" :color="activePortfolio === 'mobileapp' ? 'indigo white--text' : ''" class="mx-5">
                        Mobile App
                    </v-chip>
                    <v-chip @click="activePortfolio = 'desktopapp'" :color="activePortfolio === 'desktopapp' ? 'indigo white--text' : ''" class="mx-5">
                        Desktop App
                    </v-chip>
              </div>
          </v-col>
          
          <slot v-if="activePortfolio === 'webapp'">          
            <v-col lg="4" v-for="(app, index) in webApps" :key="index">
                <v-card>
                    <v-img
                    src='./../assets/app.jpg'
                    class="white--text align-end"
                    gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                    height="200px"
                    >
                        <v-card-title>{{app.title}}</v-card-title>
                    </v-img>
                </v-card>
            </v-col>
          </slot>

          <slot v-if="activePortfolio === 'mobileapp'">          
            <v-col lg="4" v-for="(app, index) in mobileApps" :key="index">
                <v-card>
                    <v-img
                    src='./../assets/app.jpg'
                    class="white--text align-end"
                    gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                    height="200px"
                    >
                        <v-card-title>{{app.title}}</v-card-title>
                    </v-img>
                </v-card>
            </v-col>
          </slot>
          
          <slot v-if="activePortfolio === 'desktopapp'">          
            <v-col lg="4" v-for="(app, index) in desktopApps" :key="index">
                <v-card>
                    <v-img
                        src='./../assets/app.jpg'
                        class="white--text align-end"
                        gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                        height="200px"
                    >
                        <v-card-title>{{app.title}}</v-card-title>
                    </v-img>
                </v-card>
            </v-col>
          </slot>

      </v-row>
  </v-container>
</template>

<script>
export default {
    name: 'Portfolio',
    data () {
        return {
            activePortfolio: 'webapp',
            webApps: [
                { title: 'Web App 1', image: '' },
                { title: 'Web App 2', image: '' },
                { title: 'Web App 3', image: '' },
                { title: 'Web App 4', image: '' },
                { title: 'Web App 5', image: '' },
                { title: 'Web App 6', image: '' }
            ],
            mobileApps: [
                { title: 'Mobile App 1', image: '' },
                { title: 'Mobile App 2', image: '' },
                { title: 'Mobile App 3', image: '' }
            ],
            desktopApps: [
                { title: 'Desktop App 1', image: '' },
                { title: 'Desktop App 2', image: '' },
                { title: 'Desktop App 3', image: '' },
                { title: 'Desktop App 4', image: '' }
            ]
        }
    }
}
</script>