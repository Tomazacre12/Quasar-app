<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>

        <q-toolbar-title class="absolute-center">
          SmackChat
        </q-toolbar-title>

      </q-toolbar>
    </q-header>



    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
import { openURL } from 'quasar';

export default defineComponent({
  computed: {
    title() {
      console.log(this.$route)
    }
  },
  methods: {
    openURL
  }
});
</script>
