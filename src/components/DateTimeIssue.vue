<template>
  <ion-page>
    <ion-content>
      <ion-label>Start:</ion-label>
      <ion-datetime
        v-model="startIsoTime"
        :min="minStartIsoIsoTime"
        :max="maxStartIsoTime"
      >
      </ion-datetime>
      <ion-datetime
        v-model="endIsoTime"
        :min="minEndIsoTime"
        :max="maxEndIsoTime"
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
      minStartIsoTime: "2022-11-02T11:14:00",
      maxStartIsoTime: "2022-11-02T12:14:00",
      startIsoTime: "2022-11-02T11:14:00",
      minEndIsoTime: "2022-11-02T11:15:00",
      maxEndIsoTime: undefined,
      endIsoTime: "2022-11-02T12:14:00",
    };
  },
});
</script>
