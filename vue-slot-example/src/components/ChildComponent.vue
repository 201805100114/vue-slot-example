<template>
  <div>
    <h3>子组件内容：</h3>

    <!-- 默认插槽 -->
    <div>
      <slot>默认内容：如果父组件没有传递内容，我会显示</slot>
    </div>

    <!-- 具名插槽 -->
    <div>
      <slot name="header">默认头部内容</slot>
    </div>

    <div>
      <slot name="footer">默认底部内容</slot>
    </div>
  </div>
</template>

<script>
export default {
  name: "ChildComponent"
}
</script>