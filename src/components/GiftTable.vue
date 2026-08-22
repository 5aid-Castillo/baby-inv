<script setup>
import { invitationData } from '../data/invitation.js'
</script>

<template>
  <section
    v-if="invitationData.giftTable.enabled"
    class="section gift-section"
  >
    <div class="gift-card">

      <div class="gift-icon">
        🎁
      </div>

      <p class="section-eyebrow">
        UN DETALLE PARA VICTORIA
      </p>

      <h2>
        {{ invitationData.giftTable.title }}
      </h2>

      <div class="gift-divider">
        <span>♡</span>
      </div>

      <p class="gift-text">
        {{ invitationData.giftTable.text }}
      </p>

      <div class="gift-store">

        <span class="store-label">
          MESA DE REGALOS
        </span>

        <strong>
          {{ invitationData.giftTable.store }}
        </strong>

        <div
          v-for="list in invitationData.giftTable.lists"
          :key="list.listNumber"
          class="gift-list"
        >
          <span class="list-number">
            Lista #{{ list.listNumber }}
          </span>

          <a
            :href="list.url"
            target="_blank"
            rel="noopener noreferrer"
            class="primary-button"
          >
            Ver mesa de regalos
          </a>
        </div>

      </div>

    </div>
  </section>
</template>