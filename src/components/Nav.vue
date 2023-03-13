<template>
  <div>
    <ul v-for="link in links" :key="link.id">
      <li>
        <a :href="link.page">{{ link.text }}</a>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    return {
      links: [
        {
          id: 0,
          text: "About",
          page: "/about",
        },
        {
          id: 1,
          text: "page 1",
          page: "/page1",
        },
        {
          id: 2,
          text: "page 2",
          page: "/page2",
        },
      ],
    };
  },
};
</script>
