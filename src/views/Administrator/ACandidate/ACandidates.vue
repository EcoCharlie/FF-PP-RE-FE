<template>
  <v-card
      class="mx-auto"
      elevation="0"
  >
    <v-card max-width="1200" class="mx-auto my-2" elevation="0">
      <v-container  class="d-flex justify-space-around mb-1">
        <v-btn color=#607D8B class="white--text">VOLVER</v-btn>
        <v-card-actions>
          <v-card-title><h1>Candidatos</h1></v-card-title>
        </v-card-actions>
        <v-dialog v-model="dialog"
                  width="500">
          <template v-slot:activator="{ on, attrs }">
            <v-btn color="red" class="white--text" v-bind="attrs"
                   v-on="on">+ AGREGAR</v-btn>
          </template>
          <v-card>
            <div align="center"><h1>Agrega Nuevo Candidato</h1></div>
            <v-container>
              <v-card
                  class="mx-10"
                  elevation="0"
              >
                <v-container>
                  <p>Nombre</p>
                  <v-col
                      cols="10"
                      md="12"
                  >
                    <v-text-field
                        label="Ingrese nombre del candidato"
                        outlined
                    ></v-text-field>
                  </v-col>
                  <p>Apellido</p>
                  <v-col
                      cols="10"
                      md="12"
                  >
                    <v-text-field
                        label="Ingrese apellido del candidato"
                        outlined
                    ></v-text-field>
                  </v-col>
                  <p>Fecha de nacimiento</p>
                  <v-col
                      cols="10"
                      md="12"
                  >
                    <v-text-field
                        label="Ingrese fecha de nacimiento"
                        outlined
                    ></v-text-field>
                  </v-col>
                  <p>Lugar de nacimiento</p>
                  <v-col
                      cols="10"
                      md="12"
                  >
                    <v-text-field
                        label="Ingrese lugar de nacimiento"
                        outlined
                    ></v-text-field>
                  </v-col>
                  <p>Profesión</p>
                  <v-col
                      cols="10"
                      md="12"
                  >
                    <v-text-field
                        label="Ingrese profesión del candidato"
                        outlined
                    ></v-text-field>
                  </v-col>
                  <p>Partido Político</p>
                  <v-col
                      cols="10"
                      md="12"
                  >
                    <v-text-field
                        label="Ingrese partido político"
                        outlined
                    ></v-text-field>
                  </v-col>
                </v-container>
                <v-container>
                  <v-file-input
                      label="+ Ingrese una imagen"
                      outlined
                      dense
                  ></v-file-input>
                </v-container>
              </v-card>
            </v-container>
            <v-container>
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn color="red" class="white--text">GUARDAR</v-btn><p class="mx-3"></p><v-btn color=#607D8B class="white--text">VOLVER</v-btn>
              </v-card-actions>
            </v-container>
          </v-card>
        </v-dialog>
      </v-container>
      <v-container  class="d-flex justify-space-around mb-1">
        <v-card
            class="mx-auto"
            max-width="360"
        >
          <v-card-title>Pedro Castillo<v-icon class="mx-2" color="grey">mdi-pencil</v-icon></v-card-title>
          <v-card-subtitle>Perú Libre</v-card-subtitle>
          <v-img
              src="@/assets/Image (4).png"
          ></v-img>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-card-subtitle>Profesión: Docente y político</v-card-subtitle>
            <v-spacer></v-spacer>
          </v-card-actions>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn text color="red">VER VISTA PREVIA</v-btn>
            <v-spacer></v-spacer>
          </v-card-actions>
        </v-card>
        <v-card
            class="mx-auto"
            max-width="360"
        >
          <v-card-title>Keiko Fujimori<v-icon class="mx-2" color="grey">mdi-pencil</v-icon></v-card-title>
          <v-card-subtitle>Fuerza Popular</v-card-subtitle>
          <v-img
              src="@/assets/Image (6).png"
          ></v-img>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-card-subtitle>Profesión: Política y administradora</v-card-subtitle>
            <v-spacer></v-spacer>
          </v-card-actions>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn text color="red">VER VISTA PREVIA</v-btn>
            <v-spacer></v-spacer>
          </v-card-actions>
        </v-card>
        <v-card
            class="mx-auto"
            max-width="360"
        >
          <v-card-title>Rafael López Aliaga<v-icon class="mx-2" color="grey">mdi-pencil</v-icon></v-card-title>
          <v-card-subtitle>Renovación Popular</v-card-subtitle>
          <v-img
              src="@/assets/Image (5).png"
              height="242"
          ></v-img>
          <v-card-actions>
            <v-card-subtitle align="center">Profesión: Político, empresario e ingeniero industrial</v-card-subtitle>
          </v-card-actions>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn text color="red">VER VISTA PREVIA</v-btn>
            <v-spacer></v-spacer>
          </v-card-actions>
        </v-card>
      </v-container>
      <v-container  class="d-flex justify-space-around mb-1">
        <v-card
            class="mx-auto"
            max-width="360"
        >
          <v-card-title>Hernando De Soto<v-icon class="mx-2" color="grey">mdi-pencil</v-icon></v-card-title>
          <v-card-subtitle>Avanza País</v-card-subtitle>
          <v-img
              src="@/assets/Image (7).png"
          ></v-img>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-card-subtitle>Profesión: Economista y político</v-card-subtitle>
            <v-spacer></v-spacer>
          </v-card-actions>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn text color="red">VER VISTA PREVIA</v-btn>
            <v-spacer></v-spacer>
          </v-card-actions>
        </v-card>
        <v-card
            class="mx-auto"
            max-width="360"
        >
          <v-card-title>Yonhy Lescano<v-icon class="mx-2" color="grey">mdi-pencil</v-icon></v-card-title>
          <v-card-subtitle>Acción Popular</v-card-subtitle>
          <v-img
              src="@/assets/Image (8).png"
          ></v-img>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-card-subtitle>Profesión: Abogado y político</v-card-subtitle>
            <v-spacer></v-spacer>
          </v-card-actions>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn text color="red">VER VISTA PREVIA</v-btn>
            <v-spacer></v-spacer>
          </v-card-actions>
        </v-card>
        <v-card
            class="mx-auto"
            max-width="360"
        >
          <v-card-title>Verónica Mendoza<v-icon class="mx-2" color="grey">mdi-pencil</v-icon></v-card-title>
          <v-card-subtitle>Juntos por el Perú</v-card-subtitle>
          <v-img
              src="@/assets/Image (9).png"
          ></v-img>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-card-subtitle>Profesión: Política, antropóloga y psicóloga</v-card-subtitle>
            <v-spacer></v-spacer>
          </v-card-actions>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn text color="red">VER VISTA PREVIA</v-btn>
            <v-spacer></v-spacer>
          </v-card-actions>
        </v-card>
      </v-container>
      <v-container  class="d-flex justify-space-around mb-1">
        <v-card
            class="mx-auto"
            max-width="360"
        >
          <v-card-title>Cesar Acuña <v-icon class="mx-2" color="grey">mdi-pencil</v-icon></v-card-title>
          <v-card-subtitle>Alianza para el Progreso</v-card-subtitle>
          <v-img
              src="@/assets/Image (10).png"
          ></v-img>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-card-subtitle>Profesión: Empresario y político</v-card-subtitle>
            <v-spacer></v-spacer>
          </v-card-actions>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn text color="red">VER VISTA PREVIA</v-btn>
            <v-spacer></v-spacer>
          </v-card-actions>
        </v-card>
        <v-card
            class="mx-auto"
            max-width="360"
        >
          <v-card-title>George Forsyth<v-icon class="mx-2" color="grey">mdi-pencil</v-icon></v-card-title>
          <v-card-subtitle>Victoria Nacional</v-card-subtitle>
          <v-img
              src="@/assets/Image (11).png"
          ></v-img>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-card-subtitle>Profesión: Político, exfutbolista y empresario</v-card-subtitle>
            <v-spacer></v-spacer>
          </v-card-actions>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn text color="red">VER VISTA PREVIA</v-btn>
            <v-spacer></v-spacer>
          </v-card-actions>
        </v-card>
        <v-card
            class="mx-auto"
            max-width="360"
        >
          <v-card-title>Daniel Urresti<v-icon class="mx-2" color="grey">mdi-pencil</v-icon></v-card-title>
          <v-card-subtitle>Podemos Perú</v-card-subtitle>
          <v-img
              src="@/assets/Image (12).png"
          ></v-img>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-card-subtitle>Profesión: Militar y político</v-card-subtitle>
            <v-spacer></v-spacer>
          </v-card-actions>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn text color="red">VER VISTA PREVIA</v-btn>
            <v-spacer></v-spacer>
          </v-card-actions>
        </v-card>
      </v-container>
    </v-card>
  </v-card>
</template>

<script>
export default {
  name: "ACandidates",
  data: () => ({
    files: [],
  }),
}
</script>

<style scoped>

</style>