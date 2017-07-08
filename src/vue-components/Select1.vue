<template>
  <div class="vcselect1">
    <div class="custom-select1_01">
    <select id="cat2">
      <option>item1</option>
      <option>item2</option>
      <option>item3</option>
      <option>item4</option>
      <option>Lorem ipsum dolor sit amet sed do eiusmod</option>
    </select>
  </div><input type="button" value="Search">
</div>
</template>
<script>
  export default {
    data () {
      return {    
      }
    },
    mounted: function () {
      console.log("Select1.vue mounted");
    }
  }
</script>