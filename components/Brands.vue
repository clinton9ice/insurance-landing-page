<template>
  <Section>
    <h5 class="text-muted">{{ title }}</h5>
    <br />
    <div class="brand-inline">
      <div v-if="!Array.isArray(brands)">Empty</div>
      <img
        v-for="(brand, index) in brands"
        :key="index"
        :src="require('../static/img/' + brand)"
        alt="brand"
        class="brands"
        v-else
      />
    </div>
    <br />
  </Section>
</template>

<script>
export default {
  name: "Brands",
  props: {
    brands: {
      type: Array,
      default: () => [
        "brands/image 2.png",
        "brands/image 7.png",
        "brands/image 8.png",
        "brands/LeadwayLogo 1.png",
        "brands/STinsurLogo 1.png",
      ],
    },
    title: {
      type: String,
      default: "Brands covered by us:",
    },
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
