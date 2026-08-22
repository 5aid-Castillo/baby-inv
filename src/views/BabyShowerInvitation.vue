<script setup>
import EventDetails from '@/components/EventDetails.vue';
import InvitationHero from '../components/InvitationHero.vue';
import DecorativeDivider from '@/components/DecorativeDivider.vue';
import { invitationData} from '../data/invitation.js'
import GiftTable from '@/components/GiftTable.vue';

</script>

<template>
    <main class="invitation">
        <InvitationHero />
         <!-- MENSAJE -->
    <section class="section message-section">

      <div class="message-card">

        <span class="section-icon">
          ✿
        </span>

        <p class="section-eyebrow">
          CON MUCHO CARIÑO
        </p>

        <h2>
          {{ invitationData.message.title }}
        </h2>

        <DecorativeDivider />

        <p class="message-text">
          {{ invitationData.message.text }}
        </p>

        <p class="baby-signature">
          {{ invitationData.baby.name }}
        </p>

      </div>

    </section>

    <!-- EVENTO -->
    <EventDetails />
    
    <!--MESA DE REGALOS-->
    <GiftTable />
    </main>
    
</template>