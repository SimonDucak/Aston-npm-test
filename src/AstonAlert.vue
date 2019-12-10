<template>
  <div>
    <div v-if="show">Hello world!</div>
  </div>
</template>

<script>
  export default {
    name: "AstonAlert",
    data() {
      return {
        show: true,
      };
    },
    mounted() {
      setTimeout(() => {
        this.show = false;
      }, 3000);
    }
  };
</script>
