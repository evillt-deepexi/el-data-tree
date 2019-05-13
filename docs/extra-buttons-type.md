自定义节点菜单(text)

  ```vue
<template>
  <el-data-tree
    :url="getUrl"
    data-path="data.payload"
    :extraButtons="extraButtons"
    extraButtonsType="text"
    :hasDelete="false"
    :hasNew="false"
  ></el-data-tree>
</template>

<script>
export default {
  data() {
    return {
      extraButtons: [
        {
          text: '#msbuild',
          atClick: (node, data) => {
            console.log('微软开发者大会', data)
          }
        },
        {
          text: '#io2019',
          atClick: () => {
            console.log('Google I/O 2019')
          }
        }
      ]
    }
  }
}
</script>

```