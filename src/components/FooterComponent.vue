<template>
  <div>
    <FooterECommerceComponent />
    <FooterLinkComponent />
    <FooterSocialComponent />
  </div>
</template>

<script>
import FooterECommerceComponent from "@/components/FooterECommerceComponent.vue";
import FooterLinkComponent from "@/components/FooterLinkComponent.vue";
import FooterSocialComponent from "@/components/FooterSocialComponent.vue";
export default {
  name: "FooterComponent",
  components: {
    FooterECommerceComponent,
    FooterLinkComponent,
    FooterSocialComponent,
  },
};
</script>

<style lang="scss" scoped></style>
