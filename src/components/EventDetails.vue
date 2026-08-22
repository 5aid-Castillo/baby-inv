<script setup>
import { invitationData } from '../data/invitation.js'
</script>

<template>
  <section id="details" class="section details-section">

    <div class="section-header">
      <span class="section-icon">♡</span>

      <p class="section-eyebrow">
        GUARDA LA FECHA
      </p>

      <h2>
        Será un día muy especial
      </h2>
    </div>

    <div class="details-grid">

      <article class="detail-card">
        <div class="detail-icon">
          ♡
        </div>

        <span class="detail-label">
          CUÁNDO
        </span>

        <h3>
          {{ invitationData.event.dateText }}
        </h3>

        <p>
          {{ invitationData.event.time }}
        </p>
      </article>

      <article class="detail-card">
        <div class="detail-icon">
          ♧
        </div>

        <span class="detail-label">
          DÓNDE
        </span>

        <h3>
          {{ invitationData.event.venue }}
        </h3>

        <p>
          {{ invitationData.event.address }}
        </p>

        <a
          :href="invitationData.event.mapsUrl"
          target="_blank"
          rel="noopener noreferrer"
          class="secondary-button"
        >
          Ver ubicación
        </a>
      </article>

    </div>

  </section>
</template>