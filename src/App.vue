<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup

import {
  CdrGrid,
  CdrText,
  CdrButton,
  CdrLink,
} from "@rei/cedar/dist/cedar.mjs";

</script>

<template>
  <div class="cdr-container">
    <cdr-grid
      class="cdrPage"
      style="
        grid-template-areas: 'logo header header header' 'content content content sidebar' 'footer footer footer footer';
      "
    >
      <div style="grid-area: logo">logo</div>
      <div style="grid-area: header">
        <cdr-text class="cdr-page__heading" tag="h1"> heading </cdr-text>
      </div>
      <div style="grid-area: content">
        <cdr-button>Hey I'm a button</cdr-button>
      </div>
      <div style="grid-area: sidebar">sidebar</div>
      <div style="grid-area: footer">footer</div>
    </cdr-grid>
  </div>
</template>

<style lang="scss">

</style>
