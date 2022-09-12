<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="font-poppins header__clr">
      <q-toolbar>

        <q-toolbar-title class="text-bold">
          LFCASH211M009
        </q-toolbar-title>

        <div style="font-size: 16px">{{ timestamp }}</div>
      </q-toolbar>
    </q-header>


    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue';
import moment from 'moment'

export default defineComponent({
  name: 'MainLayout',

  components: {
    
  },

  data: () => 
    ({
      timestamp: "",
    }),
    created() 
    {
        setInterval(this.getNow, 1000);
    },
    methods: {
      getNow: function() 
      {
        // return moment().format('h:mm A');
        const time = moment().format('h:mm A');
        this.timestamp = time;
      },

    },

})
</script>


<style>
.header__clr {
  background: rgba( 0, 50, 87, 0.1);
  box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
  backdrop-filter: blur( 8.5px );
  -webkit-backdrop-filter: blur( 8.5px );
}
</style>