# 主题标签动物图片说明

## 目录说明
此目录用于存放主题标签卡片上显示的可爱动物图片。

## 当前配置的标签图片

在 `themes/paper/templates/tags.ejs` 文件中，已为以下标签配置了对应的图片：

1. **编程** → `rabbit.png` (兔子)
2. **社会** → `fox.png` (狐狸)
3. **我也略懂法律** → `cat.png` (猫)
4. **历史** → `dog.png` (狗)

## 如何添加新标签的图片

### 方法一：为新标签配置特定图片

1. 将你的动物图片放入 `/images/animals/` 目录，例如：`panda.png`

2. 打开 `themes/paper/templates/tags.ejs` 文件

3. 在 `tagConfig` 对象中添加新标签的配置：

```javascript
tagConfig['你的新标签名称'] = {
  image: themeConfig.domain + '/images/animals/panda.png',
  description: '你的标签描述',
  color: 'primary'  // 可选：'primary', 'secondary', 或 'tertiary'
};
```

### 方法二：使用默认图片（自动分配）

如果你不配置特定图片，系统会自动从以下默认图片列表中循环选择：

- `rabbit.png` (兔子)
- `fox.png` (狐狸)
- `cat.png` (猫)
- `dog.png` (狗)
- `panda.png` (熊猫)
- `koala.png` (考拉)
- `tiger.png` (老虎)
- `lion.png` (狮子)
- `frog.png` (青蛙)
- `pig.png` (猪)
- `cow.png` (牛)
- `bear.png` (熊)

## 图片要求

- **格式**：PNG、JPG、JPEG、SVG 均可
- **尺寸**：建议 200x200px 或更大（正方形）
- **风格**：可爱、卡通风格的动物图片
- **背景**：建议使用透明背景或浅色背景

## 图片获取建议

你可以从以下网站获取免费的可爱动物图片：
- [Flaticon](https://www.flaticon.com/) - 搜索 "cute animal"
- [Freepik](https://www.freepik.com/) - 搜索 "cute animal icon"
- [Unsplash](https://unsplash.com/) - 搜索 "cute animal"
- 使用 AI 生成工具创建自定义动物图片

## 注意事项

- 图片文件名区分大小写
- 确保图片路径正确（相对于网站根目录）
- 如果图片加载失败，会显示默认的 🐾 表情符号作为备用


