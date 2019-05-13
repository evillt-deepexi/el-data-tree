自定义节点文本内容

 ```vue
<template>
  <el-data-tree :url="getUrl" data-path="data.payload">
    <span slot="node-text" slot-scope="{ row }">
      <el-tag size="mini">{{ row.id }}</el-tag>
      {{ row.name }}
    </span>
  </el-data-tree>
</template>
```