<template>
  <v-timeline :align-top="alignTop" :dense="dense">
    <v-timeline-item
      :fill-dot="fillDot"
      :hide-dot="hideDot"
      :icon="icon ? 'mdi-star' : ''"
      :icon-color="iconColor ? 'deep-orange' : ''"
      :left="left"
      :right="right"
      :small="small"
    >
      <span slot="opposite">2018-</span>
      <v-card class="elevation-2">
        <v-card-title class="headline">Dohop</v-card-title>
        <v-card-text>
          In 2018, after joining again full time I started taking more
          responsibility in terms of management. I joined a team working on
          three new interlining platforms with airlines in Asia. It took some
          time to get used to not "just" being a developer and learning new
          things managing people and tasks, and that is still an ongoing process
          but I really enjoy it. In 2019 two of the three platforms went live.
        </v-card-text>
      </v-card>
    </v-timeline-item>
    <v-timeline-item
      :fill-dot="fillDot"
      :hide-dot="hideDot"
      :icon="icon ? 'mdi-star' : ''"
      :icon-color="iconColor ? 'deep-orange' : ''"
      :left="left"
      :right="right"
      :small="small"
    >
      <span slot="opposite">2018</span>
      <v-card class="elevation-2">
        <v-card-title class="headline">Rainmaking</v-card-title>
        <v-card-text>
          Software Engineer working in React-Native, Scala and other things
        </v-card-text>
      </v-card>
    </v-timeline-item>
    <v-timeline-item
      :fill-dot="fillDot"
      :hide-dot="hideDot"
      :icon="icon ? 'mdi-star' : ''"
      :icon-color="iconColor ? 'deep-orange' : ''"
      :left="left"
      :right="right"
      :small="small"
    >
      <span slot="opposite">2016 & 2018</span>
      <v-card class="elevation-2">
        <v-card-title class="headline">JSConf Iceland Organizer</v-card-title>
        <v-card-text>
          JConf Iceland is a conference based on JSConf US. The JSConf
          conferences have gone all around the world bringing people and their
          love for Javascript together. It was hosted in 2016 with huge succes:
          https://www.youtube.com/watch?v=jX8bMHTD5WA and again in 2018. The
          focus of the conference was JavaScript, techonlogy and diveristy.
        </v-card-text>
      </v-card>
    </v-timeline-item>
    <v-timeline-item
      :fill-dot="fillDot"
      :hide-dot="hideDot"
      :icon="icon ? 'mdi-star' : ''"
      :icon-color="iconColor ? 'deep-orange' : ''"
      :left="left"
      :right="right"
      :small="small"
    >
      <span slot="opposite">2015-2018</span>
      <v-card class="elevation-2">
        <v-card-title class="headline">Dohop</v-card-title>
        <v-card-text>
          First year I worked full time only doing frontend work. We migrated
          the old Python/Django framework over to React in early 2015. While
          studying I worked part time doing frontend.
        </v-card-text>
      </v-card>
    </v-timeline-item>
    <v-timeline-item
      :fill-dot="fillDot"
      :hide-dot="hideDot"
      :icon="icon ? 'mdi-star' : ''"
      :icon-color="iconColor ? 'deep-orange' : ''"
      :left="left"
      :right="right"
      :small="small"
    >
      <span slot="opposite">2014</span>
      <v-card class="elevation-2">
        <v-card-title class="headline">Dohop</v-card-title>
        <v-card-text>
          SWorking as a backend/frontend web developer at Nepal for the summer.
          It include working in Visual Studio, MSSQL, ASP .NET, C# and using
          SVN.
        </v-card-text>
      </v-card>
    </v-timeline-item>
  </v-timeline>
</template>
<script>
export default {};
</script>

<style></style>
