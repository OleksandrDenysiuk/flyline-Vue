<template>
  <div class="hero">
    <div class="hero__title">
      <slot name="title"></slot>
    </div>
    <div class="hero__description">
      <slot name="description"></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: "Hero"
};
</script>

<style lang="scss">
.hero {
  display: flex;
  flex-flow: column nowrap;
  justify-content: center;
  align-items: center;
  flex-grow: 1;
  padding: 3.5rem 0;
  color: #fff;
  background-color: #0e3178;
  border-radius: 1rem;

  &__title {
    padding-bottom: 0.5rem;
    font-size: 2rem;
  }

  &__description {
    width: 38rem;
    font-size: 0.75rem;
    line-height: 1.8;
    text-align: center;
  }
}
</style>
