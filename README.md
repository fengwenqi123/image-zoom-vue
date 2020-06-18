# image-zoom-vue

>A magnifying glass assembly of Vue

### How to use?
```bash
npm i image-zoom-vue -S
```

### Example

```vue
<template>
    <magnifier :options="magnifierOptions"></magnifier>
</template>

<script>
import magnifier from 'image-zoom-vue'

  export default {
    components: {
      magnifier
    },
    data() {
      return {
        magnifierOptions: {
          width: 200,
          height: 200,
          borderSize: 2,
          borderColor: '#666666',
          shape: '',
          src: '../src/back.png',
          srcLarge: '../src/back.png'
        }
      }
    }
  }
</script>
```

### Options
|    Property    |    Description   |   type   |	default	|
| -----------------  | ---------------- | :--------: | :----------: |
| width       | 放大镜宽度 |Number| 200 |
| height         | 放大镜高度 |Number | 200 |
| borderSize  | 放大镜边框尺寸 | Number | 2 |
| borderColor     | 放大镜边框颜色 | String | #666666 |
| shape     | 放大镜形状（circular/square） | String | circular |
| src     | 缩略图地址 | String | . |
| srcLarge     | 高清图地址 | String | , |

注：外层div需要设置width和height，以便撑开图片
