<script setup lang="ts">
import NodeList from "@/components/NodeList.vue";
import type TopicNode from "@/interfaces/TopicNode";

const nodes: Array<TopicNode> = [
  {
    title: "Programming",
    description:
      "Programming is an activity in which skilled users develop computer software.",
    id: "A",
  },
  {
    title: "Art",
    description:
      "Art is an activity dedicated to creating a scene that conveys a certain emotion.",
    id: "B",
  },
];
</script>

<template>
  <NodeList :topic-nodes="nodes" />
</template>
