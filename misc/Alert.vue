
<template>
  <q-dialog v-model="alert">
    <q-card>
      <q-card-section style="text-align:center">
        <div class="text-h6">Alert</div>
      </q-card-section>

      <q-card-section>Updated successfully</q-card-section>

      <q-card-actions align="right">
        <q-btn flat label="OK" color="primary" v-close-popup />
      </q-card-actions>
    </q-card>
  </q-dialog>
</template>

<script>
export default {
  name: "Loading"
};
</script>