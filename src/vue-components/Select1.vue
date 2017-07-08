<template>
  <div class="vcselect1">
    <div class="custom-select1_01">
    <select id="cat2" v-model="selected">
      <option v-for="i in options" v-bind:value="i"
      v-on:click="switchCategory(i.itemName)">
        {{ i.itemName }}
      </option>
    </select>
  </div><input type="button" value="GO!" v-on:click="switchCategory(selected.itemName)">
</div>
</template>
<script>
  export default {
    data () {
      return {    
        selected: {itemName: "item1"},
        options: [
          {
            itemName: "item1"
          },
          {
            itemName: "item2"
          },
          {
            itemName: "item3"
          }
        ]
      }
    },
    mounted: function () {
      console.log("Select1.vue mounted");
    },
    methods: {
      switchCategory: function(item) {
        console.log(item);
      }
    }
  }
</script>