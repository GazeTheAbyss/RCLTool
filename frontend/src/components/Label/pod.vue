<template>
  <div class="label-pod"
        :style="{ 'border-color': color }">
    <div class="circle"
          :style="{ 'border-color': color }"></div>
    <div class="title"
          :style="{ 'color': color }">{{content}}</div>
  </div>
</template>

<script>
export default {
  name: 'LabelPod',
  props: {
    content: String,
    color: String
  }
}
</script>

<style scoped>
.label-pod {
  display: flex;
  padding: 4px 8px;
  border: 1px solid;
  font-size: 11px;
  border-radius: 4px;
  margin: 0px 5px 5px 0px;
  flex-shrink: 0;
}

.circle {
  border: 2px solid;
  width: 12px;
  height: 12px;
  border-radius: 100%;
  margin-right: 5px;
}
</style>
