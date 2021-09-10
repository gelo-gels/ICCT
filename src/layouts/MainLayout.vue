<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="font-poppins" style="background-color: #003b66">
      <q-toolbar>

        <q-toolbar-title class="text-bold">
          OLSHM9
        </q-toolbar-title>

        <div style="font-size: 10px">ICCT, CAINTA</div>
      </q-toolbar>
    </q-header>


    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'MainLayout',

  components: {
    
  },

})
</script>
