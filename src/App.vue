<template>
  <div id="app">
    <SideBar :marks="marks" />
  </div>
</template>

<script>
import SideBar from "./components/SideBar.vue";

export default {
  name: "App",
  data() {
    return {
      marks: [
        {
          group: "group 1",
          marks: [
            {
              open: false,
              url: "https://urlname.com",
              image: "httpUrlImage",
              description: "lorem ipsum is a insert from latin",
            },
            {
              open: true,
              url: "https://urlname.com",
              image: "httpUrlImage",
              description: "lorem ipsum is a insert from latin",
            },
            {
              open: false,
              url: "https://urlname.com",
              image: "httpUrlImage",
              description: "lorem ipsum is a insert from latin",
            },
          ],
        },
        {
          group: "group 2",
          marks: [
            {
              url: "https://urlname.com",
              image: "httpUrlImage",
              description: "lorem ipsum is a insert from latin",
            },
            {
              url: "https://urlname.com",
              image: "httpUrlImage",
              description: "lorem ipsum is a insert from latin",
            },
            {
              url: "https://urlname.com",
              image: "httpUrlImage",
              description: "lorem ipsum is a insert from latin",
            },
          ],
        },
        {
          group: "group 3",
          marks: [
            {
              url: "https://urlname.com",
              image: "httpUrlImage",
              description: "lorem ipsum is a insert from latin",
            },
            {
              url: "https://urlname.com",
              image: "httpUrlImage",
              description: "lorem ipsum is a insert from latin",
            },
            {
              url: "https://urlname.com",
              image: "httpUrlImage",
              description: "lorem ipsum is a insert from latin",
            },
          ],
        },
      ],
    };
  },
  components: {
    SideBar,
  },
};
</script>

<style>
body {
  margin: 0;
}
</style>
