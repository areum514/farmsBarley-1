<template>
  <div class="page-container">
      <md-app>
        <md-app-toolbar class="md-primary fb_header">
          <md-button class="md-icon-button" @click="back()">
            <md-icon>arrow_back</md-icon>
          </md-button>
          <p class="md-title" style="padding-left:20px;">
              Farms Barley Pizza

          </p>
        </md-app-toolbar>
      </md-app>
  </div>

</template>

<script>
export default {
  name: 'main-header',
  methods: {
    back: function() {
      console.log("back");
      history.back();
    }
  }
}
</script>

<style scoped>
  .md-app {
    max-height: 400px;
    border: 1px solid rgba(#000, .12);
    text-align: center;
  }

  .fb_header {
    background-color: #eecb77;
  }

  /* .md-drawer {
    width: 230px;
    max-width: calc(100vw - 125px);
  } */
</style>
