<template>
<v-container>
    <v-row >
        <v-col cols="12" sm="4" md="4" lg="4" v-for="perrito in perritos" :key="perrito.nombre"><v-card
        class="mx-auto"
        max-width="400"
        >
        <v-img
        class="white--text align-end"
        height="200px"
        :src="perrito.imagen"
        >
        <v-card-title>Top 10 Best Friends</v-card-title>
        </v-img>

        <v-card-subtitle class="pb-0" >
        {{perrito.nombre}}
        </v-card-subtitle>

        <v-card-text class="text--primary">
        <div>Whitehaven Beach</div>

        <div>Whitsunday Island, Whitsunday Islands</div>
        </v-card-text>

        <v-card-actions>
        <v-btn
        color="orange"
        text
        >
        Share
        </v-btn>

        <v-btn
        color="orange"
        text
        >
        Explore
        </v-btn>
        </v-card-actions>
    </v-card>
  </v-col>
</v-row>
</v-container>
</template>

<script>
export default {
    name: 'component-grid',
    // props: {},
    data () {
        return{
            perritos:[
            {
            id: 1, 
            nombre:'Jackie',
            imagen:'https://placedog.net/640/480?id:2'
            },
            {
            id: 2, 
            nombre:'Aquiles',
            imagen:'https://placedog.net/640/480?id:3'
            },
              {
            id: 3, 
            nombre:'Princess',
            imagen:'https://placedog.net/640/480?id:4'
            },
              {
            id: 4, 
            nombre:'Mockita',
            imagen:'https://placedog.net/640/480?id:5'
            },
              {
            id: 5, 
            nombre:'Blackie',
            imagen:'https://placedog.net/640/480/sepia?id:3'
            },
              {
            id: 6, 
            nombre:'Alú',
            imagen:'https://placedog.net/640/480/g?id:4'
            },

        ]   
        }

    },
    // computed: {},
    methods: {
        // -- Metodos
    },
    // components: {},
}
</script>

<style scoped>
    
</style>