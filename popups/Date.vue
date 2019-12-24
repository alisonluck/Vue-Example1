<template>
  <div class="row q-mb-sm">
    <q-input
      filled
      class="q-pa-sm"
      label="Date"
      :value="date"
      @input="$emit('update:date', $event)"
    >
      <template v-slot:append>
        <q-icon
          v-if="date"
          @click="$emit('clear')"
          name="close"
          color="primary"
          class="cursor-pointer"
        />
        <q-icon name="event" class="cursor-pointer">
          <q-popup-proxy>
            <q-date :value="date" @input="$emit('update:date', $event)" />
          </q-popup-proxy>
        </q-icon>
      </template>
    </q-input>
  </div>
</template>

<script>
export default {
  props: ["date"]
};
</script>