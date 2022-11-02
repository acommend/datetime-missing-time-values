<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <DateTimeIssue />
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { IonPage, IonContent } from "@ionic/vue";
import DateTimeIssue from "@/components/DateTimeIssue.vue";

export default defineComponent({
  name: "Tab1Page",
  components: { DateTimeIssue, IonContent, IonPage },
});
</script>
