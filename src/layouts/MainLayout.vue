<template>
  <q-layout view="hHh lpR fFf">

    <q-header reveal elevated class="bg-primary text-white" height-hint="98">

      <q-tabs
         v-model="tab"
        align="justify"
        >
         <q-toolbar-title>
          <q-avatar>
            <img src="https://cdn.quasar.dev/logo/svg/quasar-logo.svg">
          </q-avatar>
          Title
        </q-toolbar-title>
        <q-route-tab to="/"><router-link to="#a1">page 1 </router-link> </q-route-tab>
        <q-route-tab to="/home"><router-link to="/#a5">page 5 </router-link> </q-route-tab>
         <q-route-tab to="/home"><router-link to="/home#a3">page 3 </router-link> </q-route-tab>
          <q-route-tab to="/home"><router-link to="/about#a6">page 6 </router-link> </q-route-tab>
        <q-route-tab to="/about" label="Page Three" />
      </q-tabs>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

  </q-layout>
</template>

<script>
export default {
  name: 'MainLayout',
  data () {
    return {
    }
  }
}
</script>
