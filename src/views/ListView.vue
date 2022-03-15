<template>
  <div id="divMenuList">
    <p>ListView</p>
    <ul>
      <li v-for="item in data1" :key="item">
        {{ item.name }}
      </li>
    </ul>
  </div>
</template>

<script>

export default {
  name: "ListView",
};

const app = Vue.createApp({
  data() {
    return {
      data1: [
        {
          id: 1,
          name: "jerry",
        },
        {
          id: 2,
          name: "ben",
        },
        {
          id: 3,
          name: "borry",
        }
      ],
    };
  },
});
app.mount("#divMenuList");
</script>
