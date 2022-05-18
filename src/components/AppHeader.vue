<template>
  <header class="header">
    <div class="header__logo">
      <img src="../assets/img/dc-logo.png" alt="" />
    </div>
    <div class="header__menu">
      <ul>
        <li
          v-for="(item, index) in links"
          :key="index"
          :class="{ active: item.active }"
        >
          <a href="#"> {{ item.text }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data: function () {
    return {
      links: [
        {
          url: "#",
          text: "CHARACTERS",
          active: false,
        },
        {
          url: "#",
          text: "COMICS",
          active: true,
        },
        {
          url: "#",
          text: "MOVIES",
          active: false,
        },
        {
          url: "#",
          text: "TV",
          active: false,
        },
        {
          url: "#",
          text: "GAMES",
          active: false,
        },
        {
          url: "#",
          text: "COLLECTIBLES",
          active: false,
        },
        {
          url: "#",
          text: "VIDEOS",
          active: false,
        },
        {
          url: "#",
          text: "FANS",
          active: false,
        },
        {
          url: "#",
          text: "NEWS",
          active: false,
        },
        {
          url: "#",
          text: "SHOP",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.header {
  width: $general-width-page;
  margin: $general-center-page;
  display: flex;
  justify-content: space-between;
  align-items: center;
  &__logo {
    img {
      width: 70%;
    }
  }
  &__menu {
    ul {
      display: flex;
      li {
        list-style: none;
        margin-left: 0.8rem;

        li.active {
          color: blue;
          border-bottom: 1px solid blue;
        }
        a {
          text-decoration: $leave-decoration-text;
          color: black;
          line-height: 5px;
        }
      }
    }
  }
}
</style>
