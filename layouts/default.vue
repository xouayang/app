<template>
  <div>
    <div v-if="$vuetify.breakpoint.mobile">
      <v-app dark>
        <v-app-bar
          :clipped-left="clipped"
          fixed
          app
          elevation="0"
          color="primary"
        >
          <div class="white--text me-4">{{ title }}</div>
          <v-text-field
            solo
            dense
            placeholder="Search"
            hide-details="auto"
            rounded
          >
            <template #append>
              <v-btn icon small color="primary" rounded>
                <v-icon class="pt-1 ps-1 text-center"> mdi-magnify </v-icon>
              </v-btn>
            </template>
          </v-text-field>
          <v-spacer />
        </v-app-bar>
        <v-footer fixed padless elevation="20">
          <v-bottom-navigation color="primary" grow>
            <v-btn>
              <span>Login</span>
              <v-icon size="28" color="primary">mdi-account-outline</v-icon>
            </v-btn>
            <v-btn>
              <span>Cart</span>
              <v-icon size="28" color="primary">mdi-cart-outline</v-icon>
            </v-btn>
            <v-btn>
              <span>English</span>
              <v-icon size="28" color="primary">mdi-translate</v-icon>
            </v-btn>
          </v-bottom-navigation>
        </v-footer>
        <v-main>
          <v-container>
            <Nuxt />
          </v-container>
        </v-main>
      </v-app>
    </div>
    <v-app v-else>
      <v-app-bar :clipped-left="clipped" fixed app color="primary">
        <v-container class="d-flex align-center">
          <v-app-bar-title class="white--text">
            {{ title }}
          </v-app-bar-title>
          <v-spacer></v-spacer>
          <v-text-field
            solo
            dense
            placeholder="Search"
            hide-details="auto"
            rounded
          >
            <template #append>
              <v-btn icon small color="primary" rounded>
                <v-icon class="pt-1 ps-1 text-center"> mdi-magnify </v-icon>
              </v-btn>
            </template>
          </v-text-field>
          <v-spacer></v-spacer>
          <div v-ripple class="text-center me-6" style="cursor:pointer">
            <div>
              <v-icon color="white" size="28">mdi-account-outline</v-icon>
            </div>
            <div class="white--text">Login</div>
          </div>
          <div v-ripple class="text-center me-6" style="cursor:pointer">
            <div><v-icon color="white" size="28">mdi-cart-outline</v-icon></div>
            <div class="white--text">Cart</div>
          </div>
          <div v-ripple class="text-center" style="cursor:pointer">
            <div><v-icon color="white" size="28">mdi-translate</v-icon></div>
            <div class="white--text">English</div>
          </div>
          <!-- <div v-ripple class="text-center" style="cursor:pointer">
            <div><v-icon color="white" size="28">mdi-white-balance-sunny</v-icon></div>
          </div> -->
          
        </v-container>
      </v-app-bar>
      <v-main>
        <v-container>
          <Nuxt />
        </v-container>
      </v-main>
      <v-footer :absolute="!fixed" app>
        <span>&copy; {{ new Date().getFullYear() }}</span>
      </v-footer>
    </v-app>
  </div>
</template>
<script>
export default {
  name: 'DefaultLayout',
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      title: 'STORES',
    }
  },
  
}
</script>