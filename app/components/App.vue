<template>
  <Page class="page" actionBarHidden="true">
    <Frame id="app">
      <Page>
        <StackLayout />
      </Page>
    </Frame>
  </Page>
</template>

<script >
  import First from "./first";
  import Second from "./second";

  export default {
    data() {
      return {};
    },
    mounted() {
      this.$navigateTo(Second, {
        frame: "app",
        animated: false
      });
    },
    components: {
      First,
      Second
    }
  };
</script>

<style scoped>
    ActionBar {
        background-color: #53ba82;
        color: #ffffff;
    }

    .message {
        vertical-align: center;
        text-align: center;
        font-size: 20;
        color: #333333;
    }
</style>
