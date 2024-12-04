<script setup>
import { ref } from "vue"

const asideItem = ref([
  {title: "邮箱系统",  id: 1},
  {title: "办公信息",  id: 2},
  {title: "图书馆",  id: 3},
  {title: "财务系统", id: 4},
  {title: "人才招聘", id: 5}
])

const activeId = ref(1)

function isActive(i) {
  return i === activeId.value
}

function setActive(i) {
  activeId.value = i
}
</script>

<template>
  <div class="container">
    <div v-for="item in asideItem" :key="item.id" :class="{active: isActive(item.id)}" @click="setActive(item.id)">
      <li>{{ item.title }}</li>
    </div>
  </div>
</template>

<style scoped>
.container {
  height: 1000px;
  width: 150px;
  background-color: #F0FFFF;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
}

.container li {
  text-align: center;
  margin-top: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  padding:10px 0;
  margin:5px 0;
  color:#3366cc;
  border:1px soild #ccc;
  transition : background-color 0.3s;
}

.active {
  background-color:#B0E0E6;
  color: #3366cc;
}
</style>