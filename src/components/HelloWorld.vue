<template>

<v-container>
    <v-row justify="space-around">
      <v-card width="650">
        <v-img
          height="350"
          :src="url"
          cover
          class="text-white"
        >
       
          <template v-slot:placeholder>
            <div class="d-flex align-center justify-center fill-height">
              <v-progress-circular
                color="grey-lighten-4"
                indeterminate
              ></v-progress-circular>
            </div>
          </template>
        </v-img>

        <v-card-text>
          <div class="font-weight-bold ms-1 mb-2">
           You got a new life
          </div>

          <v-timeline density="compact" align="start">
            <v-timeline-item
              v-for="message in messages"
              :key="message.time"
              :dot-color="message.color"
              size="x-small"
            >
              <div class="mb-4">
                <div class="font-weight-normal">
                  <strong>{{ message.from }}</strong> @{{ message.time }}
                </div>
                <div>{{ message.message }}</div>
              </div>
            </v-timeline-item>
          </v-timeline>
          <v-card-actions>

            <v-btn @click="$event => recargaImagen()" color="black">
              RELOAD
            </v-btn>
            
          </v-card-actions>
        </v-card-text>
      </v-card>
    </v-row>
  </v-container>
</template>

<script setup>
  import { ref } from 'vue';
    const messages = ref ([]);
    const url = ref ("https://i.pinimg.com/564x/8f/d6/87/8fd687e6e6088c9b60e2e8dabcb7e6a7.jpg"); 
    messages.value = [
        {
          message: 'I am bothering you?',
          color: 'black',
        },
       ];

        function recargaImagen(){
         fetch ("https://picsum.photos/650/350?grayscale") //https://random.imagecdn.app/500/150
        .then (r => {
          console.log(r);
          url.value=r.url});
     }
  </script>    
