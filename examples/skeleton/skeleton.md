:: BASE_DOC ::

## API

### Skeleton Props

名称 | 类型 | 默认值 | 说明 | 必传
-- | -- | -- | -- | --
animation | String | - | 动画效果，有「渐变加载动画」和「闪烁加载动画」两种。值为空则表示没有动画。可选项：gradient/flashed | N
loading | Boolean | - | 是否为加载状态，如果是则显示骨架图，如果不是则显示加载完成的内容 | N
rowCol | Array | [1, 1, 1, { width: '70%' }] | 高级设置，用于自定义行列数量、宽度高度、间距等。【示例一】，`[1, 1, 2]` 表示输出三行骨架图，第一行一列，第二行一列，第三行两列。【示例二】，`[1, 1, { width: '100px' }]` 表示自定义第三行的宽度为 `100px`。【示例三】，`[1, 2, [{ width, height }, { width, height, marginLeft }]]` 表示第三行有两列，且自定义宽度、高度、尺寸（圆形或方形使用）、间距、内容等。TS 类型：`SkeletonRowCol`。[通用类型定义](https://github.com/Tencent/tdesign-vue/blob/develop/src/common.ts)。[详细类型定义](https://github.com/Tencent/tdesign-vue/tree/develop/src/skeleton/type.ts) | N
theme | String | text | 快捷定义骨架图风格，有基础、头像组合等，具体参看代码示例。可选项：text/avatar/paragraph/avatar-text/tab/article | N
