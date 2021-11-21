<script setup lang="ts">
defineProps<{
  links: string
}>()
</script>

<template>
  <div>
    <header>
      <slot />
      <component :is="links" />
    </header>
    <hr />
  </div>
</template>

<style scoped>
header {
  display: grid;
  grid-template-areas:
    "title nav"
    "hr hr";
}
::slotted {
  grid-area: title;
}
:deep(ul) {
  grid-area: nav;
  display: flex;
  justify-content: right;
  align-items: flex-end;
}
:deep(ul > li) {
  display: inline-block;
  margin: 10px;
}
hr {
  grid-area: hr;
  margin-bottom: 40px;
}
</style>
