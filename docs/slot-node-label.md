自定义节点文本内容

 ```vue
<template>
  <el-data-tree :url="getUrl" data-path="data.payload">
    <span slot="node-label" slot-scope="{ data }">
      <el-tag size="mini">{{ data.id }}</el-tag>
      {{ data.name }}
    </span>
  </el-data-tree>
</template>
```