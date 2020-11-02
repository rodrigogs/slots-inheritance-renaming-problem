<template>
  <div id="app">
    <h3>Inherited slots works</h3>
    <ComponentInheritingSlots>
      <template v-slot:slot1> Replaced slot 1 </template>
      <template v-slot:slot2> Replaced slot 2 </template>
    </ComponentInheritingSlots>
    <h3>Inherited and renamed slots doesn't</h3>
    <ComponentInheritingAndRenamingSlots>
      <template v-slot:renamed-slot1> It's not working 1 </template>
      <template v-slot:renamed-slot2> It's not working 2 </template>
    </ComponentInheritingAndRenamingSlots>
  </div>
</template>

<script>
import ComponentInheritingSlots from "@/components/ComponentInheritingSlots";
import ComponentInheritingAndRenamingSlots from "@/components/ComponentInheritingAndRenamingSlots";

export default {
  name: 'App',
  components: {
    ComponentInheritingSlots,
    ComponentInheritingAndRenamingSlots,
  }
}
</script>
