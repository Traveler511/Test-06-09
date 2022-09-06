<template>
  <div class="button" :style="{backgroundColor: bgColor}">
    <span class="button__text" >{{ text }}</span>
  </div>
</template>

<script>
export default {
  name: 'Button',
  props: {
    text: {
      type: String,
      default: ""
    },
    bgColor: {
      type: String,
      default: "black"
    }
  }
}
</script>

<style scoped lang="scss">

.button {
  cursor: pointer;
  transition: 0.2s;
  padding: 9px 17px;
  border-radius: 6px;

  &:hover {
    @media (min-width: 376px) {
      transform: scale(1.1);
    }
  }

  &__text {
    font-size: 16px;
    color: white;
  }
}


</style>
