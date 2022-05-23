<script setup lang="ts">
import type TopicNode from "@/interfaces/TopicNode";

const props = defineProps<{
  topicNodes: Array<TopicNode>;
}>();
</script>

<template>
  <div v-for="node in props.topicNodes" :key="node.id" class="list-item">
    <div class="list-item-title">
      {{ node.title }}
    </div>
    <div class="list-item-description">
      {{ node.description }}
    </div>
  </div>
</template>

<style scoped>
.list-item {
  width: calc(100% - 16px);
  border-radius: 10px;
  box-sizing: border-box;
  border: 1px solid #aaaaaa;
  padding: 8px;
  margin: 8px;
  /* box-shadow: 0px 0px 4px 0px #000000; */
}
.list-item-title {
  font-size: 1.35rem;
  color: #363636;
}
.list-item-description {
  font-size: 1.1rem;
  color: #6a6a6a;
}
</style>
