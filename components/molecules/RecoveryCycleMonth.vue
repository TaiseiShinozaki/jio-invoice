<template>
  <v-container fluid>
    <v-row align="center">
      <v-col
        class="d-flex"
        cols="12"
        sm="6"
      >
        <v-select
          :items="items"
          label="回収サイクル"
        ></v-select>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    items: ['当月', 'Bar', 'Fizz', 'Buzz'],
  }),
}
</script>