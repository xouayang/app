<template>
  <div class="mt-10">
    <v-card class="mt-5 pa-2" elevation="0">
      <div class="d-flex">
        <div class="d-flex align-center">
          <v-btn fab small color="error">
            <v-icon color="white">mdi-fire</v-icon>
          </v-btn>
          <div v-if="$vuetify.breakpoint.mobile">
             <div class="ms-2 caption"> Discounted productts</div>
          </div>
             <div class="ms-4" v-else> Discounted productts</div>
        </div>
        <v-spacer></v-spacer>
        <div class="d-flex align-center">
          <div class="me-1 caption" v-if="$vuetify.breakpoint.mobile">See more</div>
          <div class="me-1 " v-else>See more</div>

          <v-btn icon small color="blue">
            <v-icon color="blue">mdi-chevron-right</v-icon>
          </v-btn>
        </div>
      </div>
      <v-row class="mt-5">
        <v-col cols="12" md="3" sm="6">
          <v-card elevation=" 4" width="400">
            <v-img
              src="https://api.olaa.la/Files/VIVOX21_CV_09.jpg"
              height="250"
              alt="image-product"
            />
            <v-card-subtitle
              >Magnetic Case Huawei P30
              <br />
              <!-- <div class="error--text mt-2">K 1,290,000</div> -->
            </v-card-subtitle>
            <v-card-actions>
              <v-btn text small color="error"> super details </v-btn>
              <v-spacer />
              <v-btn text small color="error"> in stock </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
        <v-col cols="12" md="3" sm="6">
          <v-card elevation="4" width="400">
            <v-img
              src="https://api.olaa.la/Files/HuaweiP30_PL_01.jpg"
              height="250"
              alt="image-product"
            />
            <v-card-subtitle
              >Magnetic Case Huawei P30
              <br />
              <!-- <div class="error--text mt-2">K 1,290,000</div> -->
            </v-card-subtitle>
            <v-card-actions>
              <v-btn text small color="error"> super details </v-btn>
              <v-spacer />
              <v-btn text small color="error"> in stock </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
        <v-col cols="12" md="3" sm="6">
          <v-card elevation="4" width="400">
            <v-img
              src="https://api.olaa.la/Files/CaseMeizuM6S_CV_01fdg.jpg"
              height="250"
              alt="image-product"
            />
            <v-card-subtitle
              >Magnetic Case Huawei P30
              <br />
              <!-- <div class="error--text mt-2">K 1,290,000</div> -->
            </v-card-subtitle>
            <v-card-actions>
              <v-btn text small color="error"> super details </v-btn>
              <v-spacer />
              <v-btn text small color="error"> in stock </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
         <v-col cols="12" md="3" sm="6">
          <v-card elevation="4" width="400">
            <v-img
              src="https://api.olaa.la/Files/SamsungGalaxyS8_CV_03.jpg"
              height="250"
              alt="image-product"
            />
            <v-card-subtitle
              >Magnetic Case Huawei P30
              <br />
              <!-- <div class="error--text mt-2">K 1,290,000</div> -->
            </v-card-subtitle>
            <v-card-actions>
              <v-btn text small color="error"> super details </v-btn>
              <v-spacer />
              <v-btn text small color="error"> in stock </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-card>
  </div>
</template>
<script>
export default {}
</script>
