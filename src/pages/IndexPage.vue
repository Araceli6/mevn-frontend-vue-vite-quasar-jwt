<template>
  <q-page padding>
    <AddLink />
    <pre>
      {{ userLink.links }}
    </pre>
    <template v-for="link of userLink.links" :key="link._id">
      <LinkCard />
    </template>
  </q-page>
</template>

<script setup>
import { useLinkStore } from 'src/stores/link-store';

//components
import AddLink from 'src/components/AddLink.vue';
import LinkCard from 'src/components/LinkCard.vue';


const userLink = useLinkStore();
</script>
