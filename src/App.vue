<template>
  <v-app>
    <nav class="navbar navbar-expand-lg navbar-dark bg-light">
      <div class="container-fluid">
        <a class="navbar-brand" style="padding-left: 127px" href="/"
          ><img src="https://i.ibb.co/fYKccrd/logo.png" width="100px"
        /></a>
        <v-row class="justify-center" style="padding-top: 30px">
          <v-col cols="8 lg-4 md-4 sm-4 xs-2 xl-4">
            <v-autocomplete
              :items="items"
              filled
              class="pa-1"
              align="center"
              label="Pretražite proizvode"
              color="black"
              rounded
              item-text="naziv"
              item-value="naziv"
              clearable
              @input="dialog = true"
            >
            </v-autocomplete>
          </v-col>

        </v-row>
      </div>
    </nav>
<v-row>

                  <v-col
                  v-for="item in items"
                  :key="item.naziv"
                  cols="12"
                  sm="6"
                  md="4"
                  lg="3"
                >
                                        <v-dialog
                      v-model="dialog"
                      fullscreen
                      hide-overlay
                      transition="dialog-bottom-transition"
                    >

                      <v-card>
                        <v-toolbar dark color="primary">
                          <v-btn icon dark @click="dialog = false">
                            <v-icon>mdi-close</v-icon>
                          </v-btn>
                        </v-toolbar>
                        <br />
                        <v-row align="center" justify="center">
                          <v-col cols="6">
                            <v-img
                              width="400px"
                              :src="item.slika"
                              class="mx-auto"
                              align="center"
                              justify="center"
                            ></v-img>
                          </v-col>

                          <v-col
                            ><v-card-text
                              ><h1>{{ item.naziv }}</h1></v-card-text
                            >
                            <v-card-text
                              ><p>
                                "Lorem ipsum dolor sit amet, consectetur
                                adipiscing elit, sed do eiusmod tempor
                                incididunt ut labore et dolore magna aliqua. Ut
                                enim ad minim veniam, quis nostrud exercitation
                                ullamco laboris nisi ut aliquip ex ea commodo
                                consequat. Duis aute irure dolor in
                                reprehenderit in voluptate velit esse cillum
                                dolore eu fugiat nulla pariatur. Excepteur sint
                                occaecat cupidatat non proident, sunt in culpa
                                qui officia deserunt mollit anim id est
                                laborum."
                              </p></v-card-text
                            >
                          </v-col>
                        </v-row>
                      </v-card>
                    </v-dialog>
                  
          </v-col>
</v-row>
    <v-main>
      <v-container> </v-container>
      <router-view />
    </v-main>
    <br />
    <v-footer padless>
      <div class="container pppv">
        <div class="row">
          <div class="col h5 ppp">
            <a href="/psi" class="navbar-brand slo1">O nama</a>
          </div>
          <div class="col h5 ppp text-right">
            <a href="/psi" class="navbar-brand slo1 text-right"
              >Preuzmi brošure</a
            >
          </div>
        </div>
      </div>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    select: null,
    hello: "",
    search: "",
    dialog: false,
    cardSelectedd: null,
    items: [
      {
        brand: "VetFood Proffesional",
        naziv: "Amylactiv Balance  30 kapsula",
        terapeutskaskupina: "sinbiotici",
        vrsta: "svi",
        slika: "/slikeproizvoda/ACID-Balance-30caps.png",
      },
      {
        brand: "VetFood Proffesional",
        naziv: "Amylactiv Balance  60 kapsula",
        terapeutskaskupina: "sinbiotici",
        vrsta: "svi",
        slika: "/slikeproizvoda/ACID-Balance-60caps.png",
      },
      {
        brand: "VetFood Proffesional",
        naziv: "Amylactiv Digest 30 kapsula",
        terapeutskaskupina: "sinbiotici",
        vrsta: "svi",
        slika: "/slikeproizvoda/ACID-Balance-30caps.png",
      },
    ],
  }),
  methods: {
    open(item) {
      this.cardSelectedd = item;
    },
    close() {
      this.cardSelectedd = null;
    },
  },
};
</script>
<style scoped>
.ppp {
  font-family: "Maven Pro", sans-serif;
}
.slo1 {
  color: rgb(0, 0, 0);
}
</style>