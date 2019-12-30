<template>
  <div class="List__item">
    <v-timeline>
      <v-timeline-item large>
        <template v-slot:icon>
          <v-avatar>
            <img src="https://oi-net.eu/images/SDU_logo_blue.png" />
          </v-avatar>
        </template>
        <template v-slot:opposite>
          <span>2018</span>
        </template>
        <v-card class="elevation-2">
          <v-card-title class="headline"
            >Master thesis: Strengthen and evolve fault tolerance in a
            microservice architecture</v-card-title
          >
          <v-card-text
            >My master thesis investigated how to strengthen fault tolerance in
            a microservice architecture that strived for high availability. The
            master thesis project was three-fold and experimented with
            increasing fault tolerance under three subjects: traceability,
            resilience and chaos engineering. The thesis was done in
            co-operation with TV2, the largest streaming services of live
            television in Denmark, but the content of the thesis is protected
            under NDA.</v-card-text
          >
        </v-card>
      </v-timeline-item>
      <v-timeline-item large>
        <template v-slot:icon>
          <v-avatar>
            <img src="https://oi-net.eu/images/SDU_logo_blue.png" />
          </v-avatar>
        </template>
        <template v-slot:opposite>
          <span>2016-2018</span>
        </template>
        <v-card class="elevation-2">
          <v-card-title class="headline">MSc Software Engineering</v-card-title>
          <v-card-text>University of Southern Denmark - GPA 4</v-card-text>
        </v-card>
      </v-timeline-item>
      <v-timeline-item>
        <template v-slot:icon>
          <v-avatar>
            <img src="http://www.ru.is/media/HR_logo_hringur_hires.jpg" />
          </v-avatar>
        </template>
        <template v-slot:opposite>
          <span>2012-2015</span>
        </template>
        <v-card class="elevation-2">
          <v-card-title class="headline">BSc Computer Science</v-card-title>
          <v-card-text>Reykjavik Univeristy</v-card-text>
        </v-card>
      </v-timeline-item>
    </v-timeline>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class Academic extends Vue {}
</script>
<style></style>
