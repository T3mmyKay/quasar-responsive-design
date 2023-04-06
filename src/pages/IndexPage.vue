<script setup>
import logo from "assets/images/Vue.js_Logo_2.svg";
import quasarImg from "assets/images/quasar-logo-vertical.svg";
</script>

<template>
  <q-page class="bg-deep-purple-1">
    <div class="row bg-primary q-pb-md">
      <div class="col">
        <div style="max-width: 650px;" class="text-center q-mx-auto">
          <div class="text-h4 text-white q-mt-xl q-pt-xl q-pb-lg">Learn fullstack development from Industry experts
          </div>
          <div class="text-white text-h6 q-px-lg q-pb-sm">Join temmy.dev community to get started
          </div>
          <q-input
            filled
            placeholder="Your email"
            color="black"
            bg-color="white"
            class="q-px-lg q-pb-lg"
          >
            <template v-slot:prepend>
              <q-icon name="email" />
            </template>
            <template v-slot:append>
              <q-btn
                size="md"
                color="purple"
                label="start learning"
              />
            </template>
          </q-input>
        </div>
      </div>
      <div class="col gt-sm">
        <q-img
          class="q-mx-auto block"
          :src="logo"
          height="400px"
        />
      </div>
    </div>
    <div class="row">
      <div class="text-h5 text-bold q-px-md q-pt-md">
        Latest lessons
      </div>
    </div>
    <div class="row">
      <div class="col-12 col-md">
        <div class="q-pa-md">
          <q-card class="my-card">
            <q-video src="https://www.youtube.com/embed/k3_tw44QsZQ?rel=0" />

            <q-card-section>
              <div class="text-h6">Our Changing Planet</div>
              <div class="text-subtitle2">by John Doe</div>
            </q-card-section>

            <q-card-section class="q-pt-none">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </q-card-section>
          </q-card>
        </div>
      </div>
      <div class="col-12 col-md">
        <div class="q-pa-md">
          <q-card class="my-card">
            <q-video src="https://www.youtube.com/embed/k3_tw44QsZQ?rel=0" />

            <q-card-section>
              <div class="text-h6">Our Changing Planet</div>
              <div class="text-subtitle2">by John Doe</div>
            </q-card-section>

            <q-card-section class="q-pt-none">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </q-card-section>
          </q-card>
        </div>
      </div>
      <div class="col-12 col-md">
        <div class="q-pa-md">
          <q-card class="my-card">
            <q-video src="https://www.youtube.com/embed/k3_tw44QsZQ?rel=0" />

            <q-card-section>
              <div class="text-h6">Our Changing Planet</div>
              <div class="text-subtitle2">by John Doe</div>
            </q-card-section>

            <q-card-section class="q-pt-none">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </q-card-section>
          </q-card>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="text-h5 text-bold q-pl-md">
        Featured Lessons
      </div>
    </div>
    <div class="row">
      <div class="col-12 col-md">
        <div class="q-pa-md">
          <q-card class="my-card">
            <div class="row">
              <div class="col-12 col-md-4 q-pa-sm">
                <q-img
                  height="340px"
                  :src="quasarImg"
                />
              </div>
              <div class="col-12 col-md-8">
                <div class="text-h5 text-bold q-pl-md q-pt-sm">Getting started with Quasar and aws frameworks
                </div>
                <div class="q-pa-md">In this course you will learn about how to setup development environments for creating multi-platform apps</div>
              </div>
            </div>
          </q-card>
        </div>
      </div>
    </div>
  </q-page>
</template>
