<template>
  <v-app>
    <v-main>
      <v-sheet>
        <v-subheader>title</v-subheader>
        <v-divider />
        <v-list max-height="400" class="overflow-auto">
          <v-list-item-group>
            <template v-for="(org, index) in list">
              <v-list-item :key="org.cid" >
               {{org.cid}}
              </v-list-item>
              <v-divider :key="index"></v-divider>
            </template>
          </v-list-item-group>
        </v-list>
      </v-sheet>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",
};
</script>
