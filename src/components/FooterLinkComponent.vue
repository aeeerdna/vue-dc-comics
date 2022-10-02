<template>
  <div class="link-area">
    <!-- Links Area -->
    <div class="container">
      <!-- Links DC COMICS & Shop -->
      <div class="link-container">
        <ul>
          <p>Dc Comics</p>
          <li v-for="link in linkAreaDcComics" :key="link.title">
            <a :href="link.link">
              {{ link.title }}
            </a>
          </li>
        </ul>

        <ul>
          <p>Shop</p>
          <li v-for="link in linkShop" :key="link.title">
            <a :href="link.link">
              {{ link.title }}
            </a>
          </li>
        </ul>
      </div>

      <!-- Links DC -->
      <div class="link-container">
        <ul>
          <p>Dc</p>
          <li v-for="link in linkDc" :key="link.title">
            <a :href="link.link">
              {{ link.title }}
            </a>
          </li>
        </ul>
      </div>

      <!-- Links Sites -->
      <div class="link-container">
        <ul>
          <p>Sites</p>
          <li v-for="link in linkSites" :key="link.title">
            <a :href="link.link">
              {{ link.title }}
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterLinks",
  data() {
    return {
      linkAreaDcComics: [
        {
          title: "Characters",
          link: "#",
        },
        {
          title: "Comics",
          link: "#",
        },
        {
          title: "Movies",
          link: "#",
        },
        {
          title: "Tv",
          link: "#",
        },
        {
          title: "Games",
          link: "#",
        },
        {
          title: "Videos",
          link: "#",
        },
        {
          title: "News",
          link: "#",
        },
      ],

      linkShop: [
        {
          title: "Shop DC",
          link: "#",
        },
        {
          title: "Shop DC Collectibles",
          link: "#",
        },
      ],

      linkDc: [
        {
          title: "Terms of use",
          link: "#",
        },
        {
          title: "Privacy policy (New)",
          link: "#",
        },
        {
          title: "Add choices",
          link: "#",
        },
        {
          title: "Advertising",
          link: "#",
        },
        {
          title: "Jobs",
          link: "#",
        },
        {
          title: "Subscription",
          link: "#",
        },
        {
          title: "Talent workshop",
          link: "#",
        },
        {
          title: "CPSC Certificates",
          link: "#",
        },
        {
          title: "Ratings",
          link: "#",
        },
        {
          title: "Shop help",
          link: "#",
        },
        {
          title: "Contact us",
          link: "#",
        },
      ],

      linkSites: [
        {
          title: "DC",
          link: "#",
        },
        {
          title: "MAD magazine",
          link: "#",
        },
        {
          title: "DC kids",
          link: "#",
        },
        {
          title: "DC Universe",
          link: "#",
        },
        {
          title: "DC Power Visa",
          link: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../styles/variable.scss";

.link-area {
  background: url(../assets/img/footer-bg.jpg);
  padding-top: 25px;
  padding-bottom: 25px;
  color: $txt-main;
  .container {
    display: flex;
  }
  .link-container {
    padding: 15px;
  }
  ul {
    list-style-type: none;
    padding-top: 25px;
    p {
      text-transform: uppercase;
      font-weight: bold;
      padding-bottom: 15px;
      font-size: 1.2rem;
    }
    li {
      padding-bottom: 2px;
      a {
        height: 100%;
        text-decoration: none;
        color: $txt-footer;
      }
    }
  }
}
</style>
