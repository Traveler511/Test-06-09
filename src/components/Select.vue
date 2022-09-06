<template>
  <div class="input">
    <p class="input__label">{{label}}</p>
    <input :placeholder="placeholder" class="input__field"/>
  </div>
</template>

<script>
export default {
  name: 'Input',
  props: {
    label: {
      type: String,
      default: ""
    },
    placeholder: {
      type: String,
      default: "black"
    }
  }
}
</script>

<style scoped lang="scss">
.input {
  &__label {
    margin: 0;
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 20px;
    color: #374151;
  }
  &__field {
    margin-top: 2px;
    padding: 9px 13px;
    border: 1px solid #D1D5DB;
    border-radius: 6px;
    max-width: 170px;
    box-sizing: border-box;
    font-size: 16px;
  }

}

</style>
