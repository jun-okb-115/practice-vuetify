<template>
  <div class="team">
    <h1 class="subheading grey--text">Team</h1>
    <v-container class="my-10 grey lighten-2">
      <v-card flat class="px-3 blue-grey lighten-5">
        <v-row>
          <v-col cols="12" md="6">
            <div class="caption grey--text">Project Title</div>
            <div>Create a new website</div>
          </v-col>
          <v-col cols="6" sm="4" md="2">
            <div class="caption grey--text">Person</div>
            <div>The Net samurai</div>
          </v-col>
          <v-col cols="6" sm="4" md="2">
            <div class="caption grey--text">Due by</div>
            <div>20th May 2020</div>
          </v-col>
          <v-col cols="2" sm="4" md="2">
            <div class="caption grey--text">Status</div>
            <div>Ongoing</div>
          </v-col>
        </v-row>
      </v-card>
    </v-container>
  </div>
</template>

<script>
export default {
  name: 'Team',
}
</script>
