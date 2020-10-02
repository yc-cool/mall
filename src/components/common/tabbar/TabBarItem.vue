<template>
  <div
    :style="activeStyle"
    @click="itemClick"
    class="tab-bar-item"
    :class="{ active: isActive }"
  >
    <slot></slot>
  </div>
</template>

<script>
export default {
  data() {
    return {
      // isActive: false,
    };
  },
  props: {
    path: String,
    activeColor: {
      type: String,
      default: "palevioletred",
    },
  },
  methods: {
    itemClick() {
      if (this.$route.path !== this.path) {
        this.$router.push(this.path);
      }
      // else{
      //   return null
      // }
    },
  },
  computed: {
    isActive() {
      return this.$route.path.indexOf(this.path) !== -1;
    },
    activeStyle() {
      return this.isActive ? { color: this.activeColor } : {};
    },
  },
};
</script>

<style>
.tab-bar-item {
  /* margin: 10px 0; */
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.active {
  color: palevioletred;
}
</style>