<template>
  <div>
    <v-card class="d-flex justify-space-between mb-6">
        <v-text-field
            v-model="newHouseWork"
            label="Új házimunka"
        ></v-text-field>
        <v-btn @click="addNewHouseWork">
          Hozzáad
        </v-btn>
    </v-card>
    <v-card>
      <v-checkbox v-for="(item, index) in houseWorkList"
                  v-bind:item="item"
                  v-bind:index="index"
                  v-bind:key="item.id"
                  :label="item"
      ></v-checkbox>
    </v-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      newHouseWork: '',
      houseWorkList: []
    }
  },
  methods: {
    addNewHouseWork: function () {
      if (this.newHouseWork !== '') {
        this.houseWorkList.push(this.newHouseWork);
        this.newHouseWork = '';
      }
    }
  }
}
</script>

<style>

</style>