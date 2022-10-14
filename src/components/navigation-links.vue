<template>
  <nav class="navigation-links-nav" v-bind:class="rootClassName">
    <router-link to="/home1" class="navigation-links-navlink">
      {{ text }}
    </router-link>
    <span class="navigation-links-text">{{ text1 }}</span>
    <span class="navigation-links-text1">{{ text2 }}</span>
    <span class="navigation-links-text2">{{ text3 }}</span>
    <span class="navigation-links-text3">{{ text4 }}</span>
    <div>Placeholder for widget timer</div>
  </nav>
</template>

<script>
export default {
  name: 'NavigationLinks',
  props: {
    rootClassName: String,
    text4: {
      type: String,
      default: 'Blog',
    },
    text3: {
      type: String,
      default: 'Team',
    },
    text1: {
      type: String,
      default: 'Features',
    },
    text2: {
      type: String,
      default: 'Pricing',
    },
    text: {
      type: String,
      default: 'About',
    },
  },
}
</script>

<style scoped>
.navigation-links-nav {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  flex-direction: row;
}
.navigation-links-navlink {
  text-decoration: none;
}
.navigation-links-text {
  margin-left: var(--dl-space-space-twounits);
}
.navigation-links-text1 {
  margin-left: var(--dl-space-space-twounits);
}
.navigation-links-text2 {
  margin-left: var(--dl-space-space-twounits);
}
.navigation-links-text3 {
  margin-left: var(--dl-space-space-twounits);
}










@media(max-width: 767px) {
  .navigation-links-nav {
    align-items: flex-start;
    flex-direction: column;
  }
  .navigation-links-navlink {
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links-text {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links-text1 {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links-text2 {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links-text3 {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
}
</style>
