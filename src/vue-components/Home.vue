<template>
  <div>
    <div id="vc_select_mount">
    </div>
  </div>
</template>
<script>
  export default {
    data () {
      return {    
      }
    },
    mounted: function () {
      this.mountSelect1();
    },
    methods: {
      mountSelect1: function() {
        const Select1 = resolve => {
          require.ensure(['./Select1.vue'], () => {
            resolve(require('./Select1.vue'))
          })
        };

        new Vue({
          el: '#vc_select_mount',
          render: h => h(Select1)
        })
      }
    }
  }
</script>