<template>
  <ion-page>
    <ion-content>
      <ion-datetime
        v-model="isoTime"
        :min="minIsoIsoTime"
        :max="maxIsoTime"
        hourCycle="h12"
      >
      </ion-datetime>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { IonPage, IonContent, IonDatetime } from "@ionic/vue";

export default defineComponent({
  name: "DateTimeIssue",
  components: {
    IonPage,
    IonContent,
    IonDatetime,
  },
  setup() {
    return {
      minIsoTime: "2022-11-02T11:14:00",
      maxIsoTime: "2022-11-02T12:14:00",
      isoTime: "2022-11-02T11:14:00",
    };
  },
});
</script>
