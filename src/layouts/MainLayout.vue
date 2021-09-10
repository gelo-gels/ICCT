<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="font-poppins" style="background-color: #003b66">
      <q-toolbar>

        <q-toolbar-title class="text-bold">
          OLSHM9
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
