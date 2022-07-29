<template>
  <button
    @click="handleClick"
    :class="[
      // 主要是控制class来控制显示不同的按钮样式
      type ? 'ice-button--' + type : '',
      'button_init',
      {
        'is-plain': plain,
        'is-circle': circle,
      },
      size,
    ]"
  >
    <!-- //使用插槽 -->
    <span v-if="$slots.default"><slot></slot></span>
  </button>
</template>

<script>
export default {
  name: "Button",
  // 使用prop自定义属性
  props: {
    // type来定义button的类型
    type: {
      type: String,
      default: "normal",
    },
    // 是否为背景白色，边框和字体同颜色的简朴按钮
    plain: Boolean,
    // 是否为圆角按钮（在这里我是做了圆角处理不是完全圆）
    circle: Boolean,
    size: {
      type: String,
      default: "normal",
    },
  },
  computed: {},
  methods: {
    handleClick(evt) {
      this.$emit("click", evt);
    },
  },
};
</script>
