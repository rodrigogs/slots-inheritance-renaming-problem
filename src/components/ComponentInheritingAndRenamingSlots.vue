<template>
  <ComponentWithSlots>
    <template v-for="(_, slot) of $scopedSlots" v-slot:[slot]="scope">
      <slot :name="`renamed-${slot}`" v-bind="scope"></slot>
    </template>
  </ComponentWithSlots>
</template>

<script>
import ComponentWithSlots from "@/components/ComponentWithSlots";

export default {
  name: 'ComponentInheritingSlots',
  components: { ComponentWithSlots },
}
</script>
