<template>
  <q-btn rounded flat style="padding: 40px;">
      <q-spinner
          color="blue"
          size="2em"
          :thickness="5"
      />
  </q-btn>
</template>

<script>
export default {
  name: "Loading"
};
</script>