<template>
  <component :is="tag" class="container">
    <slot />
  </component>
</template>

<script>
export default {
  name: 'ObjectContainer',
  props: {
    tag: {
      type: String,
      default: 'div'
    }
  }
}
</script>

<style lang="scss">
.container {
  margin: 0 auto;
  max-width: 1024px;
  padding: 0 1rem;

}
</style>
