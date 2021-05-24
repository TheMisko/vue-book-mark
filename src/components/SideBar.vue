<template>
  <div class="sidebar-container">
    <div class="marks-group" v-for="(mark, index) in marks" :key="mark.group">
      {{ mark.group }} {{ index }}
      <div v-if="(mark.open = true)">
        <div v-for="groupMark in mark.marks" :key="groupMark.url">
          {{ groupMark.url }}
        </div>
      </div>
      <div v-else>yoo</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SideBar",
  props: ["marks"],
};
</script>

<style scoped>
.sidebar-container {
  width: 17vw;
  background-color: aquamarine;
  height: 100vh;
}
.marks-group {
  height: 10vh;
  margin-bottom: 15px;
  background-color: bisque;
}
</style>
