<template>
  <div class="container">
    <header>
      <!-- Logo DC -->
      <div id="logo">
        <img src="../assets/img/dc-logo.png" alt="DC Comics Logo" />
      </div>

      <!-- Menù navigazione -->
      <nav>
        <ul>
          <li v-for="link in links" :key="link.title">
            <a :href="link.link" :class="{ active: link.active }">
              {{ link.title }}
            </a>
          </li>
        </ul>
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  name: "HeaderComponent",
  data() {
    return {
      links: [
        {
          title: "Characters",
          link: "#",
          active: false,
        },
        {
          title: "Comics",
          link: "#",
          active: true,
        },
        {
          title: "Movies",
          link: "#",
          active: false,
        },
        {
          title: "Tv",
          link: "#",
          active: false,
        },
        {
          title: "Games",
          link: "#",
          active: false,
        },
        {
          title: "Collectibles",
          link: "#",
          active: false,
        },
        {
          title: "Videos",
          link: "#",
          active: false,
        },
        {
          title: "Characters",
          link: "#",
          active: false,
        },
        {
          title: "Fans",
          link: "#",
          active: false,
        },
        {
          title: "News",
          link: "#",
          active: false,
        },
        {
          title: "Shop",
          link: "#",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../styles/variable.scss";
header {
  display: flex;
  justify-content: space-between;
  margin-top: 20px;
  margin-bottom: 20px;
}

img {
  width: 75%;
}

ul {
  display: flex;
  height: 100%;
  list-style-type: none;
  text-transform: uppercase;
  font-weight: bold;
  font-size: 0.7rem;
  li {
    height: 100%;
    padding: 0px 10px;
    a {
      display: flex;
      height: 100%;
      align-items: center;
      text-decoration: none;
      color: $txt-header;
      &.active {
        border-bottom: 3px solid $bg-dc-blue;
      }
    }
  }
}
</style>
