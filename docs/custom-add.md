自定义的添加按钮

```vue
<template>
  <el-data-tree v-bind="$data" :url="getUrl" has-title title="自定义的添加按钮">
    <el-button slot="add" size="mini" type="primary">新增</el-button>
  </el-data-tree>
</template>

<script>
export default {
  data() {
    return {
      dataPath: 'data.payload'
    }
  },
}
</script>

```