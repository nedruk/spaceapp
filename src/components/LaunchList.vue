<template>
  <v-list two-line>
    <template v-for="n in 3">
      <v-list-item :key="n">
        <v-list-item-avatar color="grey darken-1">
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title class="text-h5 mb-1">Launch {{ n }}</v-list-item-title>

          <v-list-item-subtitle>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nihil repellendus distinctio similique
          </v-list-item-subtitle>

          <v-card>

            <v-card-text>
              <v-row align="center">
                <v-col cols="4">
                  <v-list-item two-line>
                    <v-list-item-content>
                      <v-list-item-title class=" mb-1">
                        Date
                      </v-list-item-title>
                      <v-list-item-subtitle>Time</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>
                <v-col class="text-h5" cols="4">
                  Mission
                </v-col>
                <v-col class="text" cols="4">
                  Details about the mission
                </v-col>
              </v-row>
            </v-card-text>
          </v-card>

        </v-list-item-content>

      </v-list-item>

      <v-divider v-if="n !== 6" :key="`divider-${n}`" inset></v-divider>
    </template>
  </v-list>
</template>