<template>
  <div id="app">
    <h1>Vue.js 插槽示例</h1>

    <!-- 使用子组件并传递插槽内容 -->
    <ChildComponent>
      <!-- 默认插槽内容 -->
      <p>这是从父组件传递的内容</p>

      <!-- 具名插槽内容 -->
      <template v-slot:header>
        <h2>这是父组件传递的头部内容</h2>
      </template>

      <template v-slot:footer>
        <h4>这是父组件传递的底部内容</h4>
      </template>
    </ChildComponent>
  </div>
</template>

<script>
import ChildComponent from "./components/ChildComponent.vue";

export default {
  name: "App",
  components: {
    ChildComponent
  }
};
</script>