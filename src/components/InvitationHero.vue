<script setup>
import { invitationData } from "../data/invitation.js";
import { ChevronDown } from "lucide-vue-next";
</script>

<template>
  <section class="hero">
    <div class="hero-overlay">
      <div class="hero-content">
        <p
          class="hero-eyebrow"
          v-motion
          :initial="{
            opacity: 0,
            y: 50,
          }"
          :enter="{
            opacity: 1,
            y: 0,
            transition: {
              duration: 1200,
            },
          }"
        >
          {{ invitationData.hero.eyebrow }}
        </p>
        <h1
          v-motion
          :initial="{
            opacity: 0,
            y: 50,
          }"
          :enter="{
            opacity: 1,
            y: 0,
            transition: {
              duration: 1200,
            },
          }"
        >
          {{ invitationData.hero.title }}
        </h1>
        <div
          class="hero-divider"
          v-motion
          :initial="{
            opacity: 0,
            y: 50,
          }"
          :enter="{
            opacity: 1,
            y: 0,
            transition: {
              duration: 1200,
            },
          }"
        >
          <span></span>
          <span>♡</span>
          <span></span>
        </div>
        <p
          class="hero-subtitle"
          v-motion
          :initial="{
            opacity: 0,
            y: 50,
          }"
          :enter="{
            opacity: 1,
            y: 0,
            transition: {
              duration: 1200,
            },
          }"
        >
          {{ invitationData.hero.subtitle }}
        </p>

        <p
          class="baby-name"
          v-motion
          :initial="{
            opacity: 0,
            y: 50,
          }"
          :enter="{
            opacity: 1,
            y: 0,
            transition: {
              duration: 1200,
            },
          }"
        >
          {{ invitationData.baby.name }}
        </p>

        <p
          class="hero-date"
          v-motion
          :initial="{
            opacity: 0,
            y: 50,
          }"
          :enter="{
            opacity: 1,
            y: 0,
            transition: {
              duration: 1200,
            },
          }"
        >
          <!-- {{ invitationData.event.dateText }} -->
        </p>

        <a
          href="#details"
          class="discover-button"
          v-motion
          :initial="{
            opacity: 0,
            y: 30,
          }"
          :enter="{
            opacity: 1,
            y: 0,
            transition: {
              duration: 1200,
              delay: 1400,
            },
          }"
        >
          <span>Descubrir invitación</span>

          <span class="discover-arrow">
            <ChevronDown />
          </span>
        </a>
      </div>
    </div>
  </section>
</template>

<style></style>
