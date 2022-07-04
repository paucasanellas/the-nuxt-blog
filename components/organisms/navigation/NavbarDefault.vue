<template>
  <Container tag="nav" class="navbar navbar--default">
    <section>
      <NuxtLink :to="{ name: 'index' }">
        <p class="title">
          <NuxtLogo /> TheNuxtBlog
        </p>
      </NuxtLink>
    </section>
    <section>
      <NuxtLink :to="{ name: 'index' }">
        Home
      </NuxtLink>
      <NuxtLink :to="{ name: 'about' }">
        About
      </NuxtLink>
    </section>
  </Container>
</template>

<script>
export default {
  name: 'NavbarDefault'
}
</script>

<style lang="scss">
@import '@/assets/styles/settings/_variables.scss';

.navbar {
  &--default {
    height: 60px;

    .title {
      font-size: $font-size-h4;
      display: flex;
      place-items: center;
    }

    a {
      font-family: $font-family-headings;
    }
  }
}
</style>
