<template>
  <q-layout view="lHh Lpr lFf">
    <q-header class="q-px-xl bg-red" elevated>
      <q-toolbar class="q-py-lg" id="toolbar">
        <q-toolbar-title id="title">
          <q-icon name="local_pizza" />
          PIZZER-IA
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />

      <div class="column items-center full-width q-gutter-y-md q-my-auto">
        <df-messenger id="dialogflow" intent="WELCOME" chat-title="¿Qué desea ordenar?" agent-id="6ac9e96a-168a-448d-9153-5e9ea552ad92"
          language-code="es"></df-messenger>
      </div>
    </q-page-container>
  </q-layout>
</template>

<script setup lang="ts">
import { defineComponent, onMounted } from "vue";
</script>

<style lang="scss">
#title {
  font-size: 1.8rem;
  font-weight: 800;
}

q-header {
  z-index: 1;
}

#toolbar {
  padding-left: 10rem;
  padding-right: 10rem;
}

#dialogflow {
margin-top: 10rem;
z-index: 1000000;
}
</style>
