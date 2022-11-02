<template>
  <ion-page>
    <ion-content>
      <ion-datetime
        v-model="startIsoTime"
        :min="minStartIsoIsoTime"
        :max="maxStartIsoTime"
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
      minStartIsoTime: "2022-11-02T11:14:00",
      maxStartIsoTime: "2022-11-02T12:14:00",
      startIsoTime: "2022-11-02T11:14:00",
    };
  },
});
</script>
