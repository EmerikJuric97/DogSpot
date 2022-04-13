<template class="bodyy">
  <v-container>
    <v-row justify="center" class="mx-auto">
      <v-col cols="4" md="2" xs="2">
        <v-app-bar color="white" bright rounded>
          <v-app-bar-nav-icon class="mx-auto" @click.stop="drawer = !drawer"
            >Filter</v-app-bar-nav-icon
          >
        </v-app-bar>
      </v-col>
    </v-row>
    <v-divider></v-divider>
    <v-navigation-drawer v-model="drawer" absolute left temporary height="300px" color="indigo lighten-4">
      <v-list nav dense >
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-expansion-panels>
            <v-expansion-panel>
              <v-expansion-panel-header
                >Vrsta životinje</v-expansion-panel-header
              >
              <v-expansion-panel-content>
                <v-list-item>
                  <v-checkbox
                    label="Svi proizvodi"
                    v-model="selectedCategory"
                    color="blue"
                    value="svi"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Proizvodi za pse"
                    v-model="selectedCategory"
                    color="blue"
                    value="pas"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Proizvodi za mačke"
                    v-model="selectedCategory"
                    color="blue"
                    value="macka"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Proizvodi za pse i mačke"
                    v-model="selectedCategory"
                    color="blue"
                    value="pasmacka"
                  ></v-checkbox>
                </v-list-item>
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-expansion-panels>
          <v-divider></v-divider>
          <v-expansion-panels>
            <v-expansion-panel>
              <v-expansion-panel-header>Brend</v-expansion-panel-header>
              <v-expansion-panel-content>
                <v-list-item>
                  <v-checkbox
                    label="VetFood Proffesional"
                    v-model="selectedCategoryyy"
                    color="blue"
                    value="svi"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="BARFeed"
                    v-model="selectedCategoryyy"
                    color="blue"
                    value="BARFeed"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Sport & Fit"
                    v-model="selectedCategoryyy"
                    color="blue"
                    value="macka"
                  ></v-checkbox>
                </v-list-item>
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-expansion-panels>
          <v-divider></v-divider>
          <v-expansion-panels>
            <v-expansion-panel>
              <v-expansion-panel-header
                >Terapeutska skupina</v-expansion-panel-header
              >
              <v-expansion-panel-content>
                <v-list-item>
                  <v-checkbox
                    label="Sinbiotici"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="sinbiotici"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Imunološki sistem"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="pas"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Regeneracija/gubitak težine"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="macka"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Potpora životinjama starije dobi"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="macka"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Bolesti srca"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="srce"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Prebiotici"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="macka"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Jetra"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="macka"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Imunološki sistem"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="macka"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Bubrezi i urinarni trakt"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="macka"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Potpora tijekom onkoloških oboljenja"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="macka"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Zglobovi"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="macka"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Oralna higijena"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="macka"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Oči"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="macka"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Gastro intestinalne bolesti"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="macka"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Za uši"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="zausi"
                  ></v-checkbox>
                </v-list-item>

                <v-list-item>
                  <v-checkbox
                    label="Koža i dlaka"
                    v-model="selectedCategoryy"
                    color="blue"
                    value="macka"
                  ></v-checkbox>
                </v-list-item>
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
    <v-data-iterator
      :items="items"
      :items-per-page.sync="itemsPerPage"
      :page.sync="page"
      :sort-by="sortBy.toLowerCase()"
      :sort-desc="sortDesc"
      hide-default-footer
    >
      <template>
        <v-row>
          <v-col
            v-for="item in filteredProizvodi"
            :key="item"
            cols="12"
            sm="6"
            md="4"
            lg="3"
          >
            <v-card>
              <v-img
                width="120"
                height="200"
                :src="item.slika"
                class="mx-auto"
              ></v-img>
              <v-card-text class="text-center" align="center" justify="center">
                {{ item.naziv }}
              </v-card-text>
              <v-dialog
                v-model="dialog"
                fullscreen
                hide-overlay
                transition="dialog-bottom-transition"
              >
                <template v-slot:activator="{ on, attrs }" class="mx-auto">
                  <v-col align="center">
                    <v-btn
                      color="white"
                      v-bind="attrs"
                      v-on="on"
                      justify="center"
                      class="mx-auto"
                      width="150px"
                      @click="open(item)"
                      
                    >
                      Više o proizvodu
                    </v-btn></v-col
                  >
                  
                </template>
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

                    <v-col open v-if="cardSelected"
                      ><v-card-text
                        ><h1>{{ cardSelected.naziv }}</h1></v-card-text
                      >
                      <v-card-text
                        ><p>
                          "Lorem ipsum dolor sit amet, consectetur adipiscing
                          elit, sed do eiusmod tempor incididunt ut labore et
                          dolore magna aliqua. Ut enim ad minim veniam, quis
                          nostrud exercitation ullamco laboris nisi ut aliquip
                          ex ea commodo consequat. Duis aute irure dolor in
                          reprehenderit in voluptate velit esse cillum dolore eu
                          fugiat nulla pariatur. Excepteur sint occaecat
                          cupidatat non proident, sunt in culpa qui officia
                          deserunt mollit anim id est laborum."
                        </p></v-card-text
                      >
                    </v-col>
                  </v-row>
                </v-card>
              </v-dialog>
            </v-card>
          </v-col>
        </v-row>
      </template>
      <template>
        <v-row>
          <v-col
            v-for="item in filteredBrand"
            :key="item"
            cols="12"
            sm="6"
            md="4"
            lg="3"
          >
            <v-card>
              <v-img
                width="120"
                height="200"
                :src="item.slika"
                class="mx-auto"
              ></v-img>
              <v-card-text class="text-center" align="center" justify="center">
                {{ item.naziv }}
              </v-card-text>
              <v-dialog
                v-model="dialog"
                fullscreen
                hide-overlay
                transition="dialog-bottom-transition"
              >
                <template v-slot:activator="{ on, attrs }" class="mx-auto">
                  <v-col align="center">
                    <v-btn
                      color="white"
                      v-bind="attrs"
                      v-on="on"
                      justify="center"
                      class="mx-auto"
                      width="150px"
                      @click="open(item)"
                    >
                      Više o proizvodu
                    </v-btn></v-col
                  >
                </template>
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
                          "Lorem ipsum dolor sit amet, consectetur adipiscing
                          elit, sed do eiusmod tempor incididunt ut labore et
                          dolore magna aliqua. Ut enim ad minim veniam, quis
                          nostrud exercitation ullamco laboris nisi ut aliquip
                          ex ea commodo consequat. Duis aute irure dolor in
                          reprehenderit in voluptate velit esse cillum dolore eu
                          fugiat nulla pariatur. Excepteur sint occaecat
                          cupidatat non proident, sunt in culpa qui officia
                          deserunt mollit anim id est laborum."
                        </p></v-card-text
                      >
                    </v-col>
                  </v-row>
                </v-card>
              </v-dialog>
            </v-card>
          </v-col>
        </v-row>
      </template>

      <template>
        <v-row>
          <v-col
            v-for="item in filteredNamjena"
            :key="item"
            cols="12"
            sm="6"
            md="4"
            lg="3"
          >
            <v-card>
              <v-img
                width="120"
                height="200"
                :src="item.slika"
                class="mx-auto"
              ></v-img>
              <v-card-text class="text-center" align="center" justify="center">
                {{ item.naziv }}
              </v-card-text>
              <v-dialog
                v-model="dialog"
                fullscreen
                hide-overlay
                transition="dialog-bottom-transition"
              >
                <template v-slot:activator="{ on, attrs }" class="mx-auto">
                  <v-col align="center">
                    <v-btn
                      color="white"
                      v-bind="attrs"
                      v-on="on"
                      justify="center"
                      class="mx-auto"
                      width="150px"
                      @click="open(item)"
                    >
                      Više o proizvodu
                    </v-btn></v-col
                  >
                </template>
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
                          "Lorem ipsum dolor sit amet, consectetur adipiscing
                          elit, sed do eiusmod tempor incididunt ut labore et
                          dolore magna aliqua. Ut enim ad minim veniam, quis
                          nostrud exercitation ullamco laboris nisi ut aliquip
                          ex ea commodo consequat. Duis aute irure dolor in
                          reprehenderit in voluptate velit esse cillum dolore eu
                          fugiat nulla pariatur. Excepteur sint occaecat
                          cupidatat non proident, sunt in culpa qui officia
                          deserunt mollit anim id est laborum."
                        </p></v-card-text
                      >
                    </v-col>
                  </v-row>
                </v-card>
              </v-dialog>
            </v-card>
          </v-col>
        </v-row>





      </template>

      <!-- Comment <template v-slot:footer>
        <v-row class="mt-2" align="center" justify="center">
          <v-spacer></v-spacer>

          <v-btn
            fab
            dark
            color="blue darken-3"
            class="mr-1"
            @click="formerPage"
          >
            <v-icon>mdi-chevron-left</v-icon>
          </v-btn>
          <v-btn fab dark color="blue darken-3" class="ml-1" @click="nextPage">
            <v-icon>mdi-chevron-right</v-icon>
          </v-btn>
          <span class="grey--text text-center">
            {{ page }} od {{ numberOfPages }}
          </span>
          <v-menu offset-y>
            <template v-slot:activator="{ on, attrs }">
              <v-btn
                dark
                text
                color="primary"
                width="250px"
                v-bind="attrs"
                v-on="on"
              >
                Proizvoda po stranici: {{ itemsPerPage }}
                <v-icon>mdi-chevron-down</v-icon>
              </v-btn>
            </template>
            <v-list>
              <v-list-item
                v-for="(number, index) in itemsPerPageArray"
                :key="index"
                @click="updateItemsPerPage(number)"
              >
                <v-list-item-title>{{ number }}</v-list-item-title>
              </v-list-item>
            </v-list>
          </v-menu>
        </v-row>
      </template> -->
    </v-data-iterator>
  </v-container>
</template> 

<script>
export default {
  data() {
    return {
      itemsPerPageArray: [4, 8, 12],
      search: "",
      filter: {},
      sortDesc: false,
      page: 1,
      itemsPerPage: 8,
      sortBy: "naziv",
      dialog: false,
      notifications: false,
      sound: true,
      widgets: false,
      zivotinjeVrsta: null,
      selectedCategory: "pas",
      selectedCategoryy: "",
      selectedCategoryyy: "",
      drawer: false,
      group: null,
      cardSelected: null,
      keys: [
        "brand",
        "naziv",
        "Fat",
        "Carbs",
        "Protein",
        "Sodium",
        "Calcium",
        "Iron",
      ],

      items: [
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "pas",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  60 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Digest 30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Anti Hairball 100 g",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Anti Herpes 60 g",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "BB & Recovery Balance 20 g ",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "BB & Recovery Balance 100 g ",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "BB & Recovery Balance Professional  2000 g ",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Brainactiv Balance 30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Cardioforce 30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Cardioforce 90 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "CBD Gold oil 500 mg  ( 1,75% ) -30 ml",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "CBD Gold oil 1500 mg ( 5% )  – 30 ml",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "For Calm 60 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "FLORActiv 100g",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Flora Balance 15 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Flora Balance 60 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Flora Balance 30 mini kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Hepatoforce 30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Hepatoforce 90 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Hepatoforce Plus 30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Hepatoforce Plus 90 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Hepatoforce Gel 30 ml",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Immunactiv Max 90 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Immunactiv Balance 60 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Immunactiv Balance za mačke 30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Intestivet Gel 15 ml",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "L-Methiocid 60 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "L-Methiocid 120 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "L-Methiocid za mačke 39 g",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "NefroActiv 60 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "No Stress Gel 15 ml",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Premium NTS Diet 115 g ",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Premium NTS Diet Immunactiv  Anticachectic 90 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Premium NTS Diet Immunactiv Anticachectic 30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Osteoarthristop 90 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Osteoarthristop Plus 90 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "PlaqueControl 60 g ",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "PlaqueControl 60 g ",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "UroForce 30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "UroForce 60 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "UroForce Plus 120 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Četkica za zube S",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Četkica za zube M",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "VisioPet ® 5 kom",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "svi",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "dsgdsf",
          terapeutskaskupina: "sinbiotici",
          vrsta: "pas",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  120 kapsula",
          terapeutskaskupina: "sinbiotici",
          vrsta: "macka",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "VetFood Proffesional",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "zausi",
          vrsta: "pas",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
        {
          brand: "BARFeed",
          naziv: "Amylactiv Balance  30 kapsula",
          terapeutskaskupina: "srce",
          vrsta: "pas",
          slika: "/slikeproizvoda/ACID-Balance-30caps.png",
        },
      ],
    };
  },
  computed: {
    numberOfPages() {
      return Math.ceil(this.items.length / this.itemsPerPage);
    },
    filteredKeys() {
      return this.keys.filter((key) => key !== "naziv");
    },
    filteredProizvodi: function () {
      var vm1 = this;
      var vrsta = vm1.selectedCategory;

      if (vrsta === "svi") {
        return vm1.items;
      } else {
        return vm1.items.filter(function (zivotinjaa) {
          return zivotinjaa.vrsta === vrsta;
        });
      }
    },
    filteredNamjena: function () {
      var vm2 = this;
      var terapeutskaskupina = vm2.selectedCategoryy;
              if (terapeutskaskupina === "svi") {
        return vm2.items;
      } else {
        return vm2.items.filter(function (zivotinjaaa) {
          return zivotinjaaa.terapeutskaskupina === terapeutskaskupina;
        });
      }
    },
    filteredBrand: function () {
      var vm3 = this;
      var brand = vm3.selectedCategoryyy;
              if (brand === "svi") {
        return vm3.items;
      } else {
        return vm3.items.filter(function (zivotinjaaaa) {
          return zivotinjaaaa.brand === brand;
        });
      }
    },
  },
  methods: {
    nextPage() {
      if (this.page + 1 <= this.numberOfPages) this.page += 1;
    },
    open(item) {
      this.cardSelected = item;
    },
        close() {
      this.cardSelected = null;
    },
    formerPage() {
      if (this.page - 1 >= 1) this.page -= 1;
    },
    updateItemsPerPage(number) {
      this.itemsPerPage = number;
    },
    svi() {
      return this.items.filter((item) => {
        return item;
      });
    },
    fruitsVeggies() {
      return this.items.filter((item) => {
        return item.category === "paks";
      });
    },
    watch: {
      group() {
        this.drawer = false;
      },
    },
  },
};
</script>
<style scoped>
.bodyy{
    font-family: 'Maven Pro', sans-serif;
}
</style>