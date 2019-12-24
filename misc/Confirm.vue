
<template>
  
    <q-card>
      <q-card-section style="text-align:center">
        <div class="text-body1">{{content}}</div>
      </q-card-section>
      <q-separator />
      <q-card-actions align="center">
        <q-btn flat label="OK" @click="agree()" color="primary" />
        <q-btn flat label="Cancel" color="primary" v-close-popup />
      </q-card-actions>
    </q-card>
  
</template>

<script>
export default {
    name: "Corfirm",
    props:['content'],
    methods:{
        agree(){
            this.$emit('confirmResult',true)
        }
    }
};
</script>