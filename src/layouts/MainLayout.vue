<script setup>
import { ref } from "vue";
import logo from "assets/images/eyelogo.jpg";

const drawer = ref(false);

const leftDrawerOpen = () => drawer.value = !drawer.value;
</script>

<template>
  <q-layout view="lHh Lpr lFf">
    <q-header>
      <q-toolbar>
        <q-toolbar-title>
          <q-img
            :src="logo"
            style="height: 50px; max-width: 50px"
          />
        </q-toolbar-title>

        <div class="gt-sm">
          <q-btn
            flat
            label="courses"
            rounded
            class="q-mr-sm"
          />
          <q-btn
            outline
            label="sign up"
            rounded
            class="q-mr-sm"
          />
          <q-btn
            outline
            label="sign in"
            rounded

          />
        </div>
        <div class="lt-md">
          <q-btn
            flat
            dense
            round
            @click="drawer = !drawer"
            icon="menu"
            aria-label="Menu"
          />


        </div>
      </q-toolbar>
    </q-header>
    <q-drawer
      v-model="drawer"
      bordered
    >
      <q-list>
        <q-item-label
          header
        >
          Essential Links
        </q-item-label>

      </q-list>
    </q-drawer>


    <q-page-container>
      <router-view />
    </q-page-container>
    <q-footer
      elevated
    >
      <q-toolbar>
       <q-space />
        &copy; temmy.dev {{new Date().getFullYear()}}
        <q-space/>
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>
