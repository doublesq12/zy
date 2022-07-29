<!--  -->
<template>
  <div>
    <div>
      <p class="explain_title">按钮类型</p>
      <Button type="normal">普通按钮</Button>
      <Button type="default">默认按钮</Button>
      <Button type="error">警告按钮</Button>
      <Button type="success">主要按钮</Button>
      <Button type="warning">警告按钮</Button>
    </div>
    <div>
      <p class="explain_title">朴素按钮</p>
      <Button plain type="normal">普通按钮</Button>
      <Button plain type="default">默认按钮</Button>
      <Button plain type="error">警告按钮</Button>
      <Button plain type="success">主要按钮</Button>
      <Button plain type="warning">警告按钮</Button>
    </div>
    <div>
      <p class="explain_title">圆角按钮</p>
      <Button circle plain type="normal">普通按钮</Button>
      <Button circle plain type="default">默认按钮</Button>
      <Button circle type="error">警告按钮</Button>
      <Button circle type="success">主要按钮</Button>
      <Button circle plain type="warning">警告按钮</Button>
    </div>
    <div>
      <p class="explain_title">按钮大小</p>
      <Button circle plain size="mini" type="normal">mini</Button>
      <Button circle plain size="small" type="default">small</Button>
      <Button circle size="normal" type="error">normal</Button>
      <Button circle size="rather" type="success">rather</Button>
      <Button circle size="big" plain type="warning">big</Button>
    </div>
    <p>自定义icon图标</p>
    <Button type="default">
      <template #default>
        <i class="iconfont icon-youjiantou"></i> 按钮
      </template>
    </Button>
  </div>
</template>

<script>
import { Button } from "@/components/button/index.js";
export default {
  components: {
    Button,
  },
  data() {
    return {};
  },
  computed: {},
  watch: {},
  methods: {
    btnclick() {
      console.log(11);
    },
  },
  //生命周期 - 创建完成（可以访问当前this实例）
  created() {},
  //生命周期 - 挂载完成（可以访问DOM元素）
  mounted() {},
};
</script>
<style scoped></style>
