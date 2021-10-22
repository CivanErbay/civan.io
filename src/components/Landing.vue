<template>
  <div class="landing">
    <div class="section landing--section-one">
      <h1>{{ content.title }}</h1>
      <img
        alt="civan erbay"
        class="landing--image"
        src="../assets/civan_erbay.png"
      />
    </div>
    <div class="section landing--section-two">
      <div class="shady"></div>
    </div>
    <div class="section landing--section-three">
      <div class="shady"></div>
    </div>
  </div>
</template>

<script>
import contentJSON from "../content.js";
export default {
  name: "Landing",
  data() {
    return {
      count: 0,
      content: contentJSON,
    };
  },
};
</script>

<style lang="scss" scoped>
.landing {
  display: flex;
  flex-direction: column;

  &--image {
    height: 50px;
  }

  .section {
    height: 33vh;
    width: 100%;
  }

  .shady {
    border: 0px solid #333;
    width: 100%;
    height: 0;
    box-shadow: 0px 3px 12px 1px rgb(0 0 0 / 75%);
  }

  &--section {
    &-one {
      background-color: rgb(255, 255, 255);
    }

    &-two {
      background-color: rgb(200, 199, 201);
    }

    &-three {
      background-color: rgb(170, 169, 170);
    }
  }
}
</style>
