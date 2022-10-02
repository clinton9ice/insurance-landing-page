<template>
  <Section>
    <h5 class="text-muted">Brands covered by us:</h5>
    <br />
    <div class="brand-inline">
      <img src="../static/img/brands/image 2.png" alt="brand" class="brands" />
      <img src="../static/img/brands/image 7.png" alt="brand" class="brands" />
      <img src="../static/img/brands/image 8.png" alt="brand" class="brands" />
      <img
        src="../static/img/brands/LeadwayLogo 1.png"
        alt="brand"
        class="brands"
      />
      <img
        src="../static/img/brands/STinsurLogo 1.png"
        alt="brand"
        class="brands"
      />
    </div>
    <br />
  </Section>
</template>

<script>
export default {
  name: "Brands",
  props: {
    brands: Array,
  },
  setup() {
    return {};
  },
};
</script>

<style scoped>
.brand-inline {
  display: flex;
  align-items: center;
  gap: 3;
  flex-shrink: 0;
  overflow: hidden;
  overflow-x: auto;
}
.brand-inline .brands {
  margin-right: 0.8rem;
  width: 100%;
  height: auto;
  object-fit: cover;
  transform: scale(0.7);
}
.brand-inline::-webkit-scrollbar {
  height: 3px;
}
</style>
