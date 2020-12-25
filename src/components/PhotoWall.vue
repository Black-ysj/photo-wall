<template>
  <div>
    <ul class="wall">
      <li v-for="(item,index) in listimg" :key="index">
        <img :src="item" alt="" />
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      listimg: [
          require('../assets/img/1.jpg'),
          require('../assets/img/2.jpg'),
          require('../assets/img/3.jpg'),
          require('../assets/img/4.jpg'),
          require('../assets/img/5.jpg'),
          require('../assets/img/6.jpg'),
          require('../assets/img/7.png'),
          require('../assets/img/8.png')
      ],
    };
  },
};
</script>

<style scoped>
.wall {
  list-style: none;
  width: 1000px;
  min-height: 500px;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}

.wall li {
  width: 230px;
}

.wall li img {
  width: 100%;
  border: 1px solid #ccc;
  padding: 5px;
  border-radius: 5px;
}
</style>