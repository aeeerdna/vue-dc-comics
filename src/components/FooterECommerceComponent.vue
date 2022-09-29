<template>
  <div class="eCommerce">
    <!-- Links eCommerce -->
    <div class="container">
      <ul>
        <li v-for="link in shopArea" :key="link.title">
          <a :href="link.link">
            {{ link.title }}
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterECommerce",
  data() {
    return {
      shopArea: [
        {
          title: "Digital Comics",
          link: "#",
        },
        {
          title: "Dc Merchandise",
          link: "#",
        },
        {
          title: "Subscription",
          link: "#",
        },
        {
          title: "Comic Shop Locator",
          link: "#",
        },
        {
          title: "Dc Power Visa",
          link: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../styles/variable.scss";
.eCommerce {
  display: flex;
  justify-content: space-between;
  background-color: $bg-dc-blue;

  ul {
    display: flex;
    height: 100%;
    list-style-type: none;
    text-transform: uppercase;
    font-weight: bold;
    li {
      height: 100%;
      padding: 0px 10px;
      a {
        display: flex;
        height: 100%;
        align-items: center;
        text-decoration: none;
        color: $txt-main;
      }
    }
  }
}
</style>
