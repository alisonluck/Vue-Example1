<template>
    
      <q-card class="full-width">
            <center>
                <q-item-label v-close-popup @click="$emit('selectMediaType', 0)" class="text-grey-8 text-h6 q-pa-sm" >
                    Image
                </q-item-label>
                <q-separator />
                <q-item-label v-close-popup @click="$emit('selectMediaType', 1)" class="text-grey-8 text-h6 q-pa-sm">
                    Video
                </q-item-label>
            </center>
      </q-card>
   
</template>

<script>
export default {
    name: 'SelectMedia',
    data(){
        return{
            prompt: false
        }
    },
    created(){

    },
    methods:{

    }
}
</script>