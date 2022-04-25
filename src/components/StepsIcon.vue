<template>
  <div class="step-icon__bg">
    <div class="step-icon__inner">
      <img src="../assets/Vector.svg" class="img-icon" />
      <img src="../assets/Vector.svg" class="img-icon" />

      <img src="../assets/Vector.svg" class="img-icon" />
      <img src="../assets/Vector.svg" class="img-icon" />
      <img src="../assets/Vector.svg" class="img-icon" />
    </div>
  </div>
</template>

<script>
export default {
  name: "StepsIcon",
};
</script>

<style scoped>
.step-icon__bg {
  display: flex;
}

.step-icon__inner {
  z-index: 999;
}
.img-icon {
  z-index: 999;
  border-radius: 50%;
  background-color: #dcdcdc;
}

</style>
