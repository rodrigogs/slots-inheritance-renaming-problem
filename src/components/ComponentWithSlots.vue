<template>
  <div style="margin-bottom: 10px">
    <div class="slot" style="background-color: aqua">
      <slot name="slot1">
        Slot 1
      </slot>
    </div>
    <div class="slot" style="background-color: coral">
      <slot name="slot2">
        Slot 2
      </slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ComponentWithSlots',
}
</script>

<style scoped>
.slot {
  text-align: center;
  padding: 10px;
}
</style>
