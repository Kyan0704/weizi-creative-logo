# Logo图片生成Prompt模板

使用 `image_gen` 工具生成logo图片时，按以下模板构造prompt。所有prompt必须为英文（图像生成模型对英文响应更稳定），并严格遵守视觉规范。

## 通用结构

```
[主体图形描述], [手法关键词], minimalist logo design, vector style, 
clean lines, [配色], [背景], centered composition, 
professional brand identity, no text, no gradient, no 3D effect, no shadow
```

## 必选后缀（每个prompt都必须包含）

```
no text, no letters, no words, no gradient, no 3D, no shadow, 
no photorealistic, no background details, pure flat vector
```

## 各手法Prompt模板

### 1. 设计减法

```
A minimalist [主体] logo formed by only [数量] essential strokes, 
reduced to absolute minimum, bare minimum representation still 
recognizable as [主体], single color black on pure white background, 
vector flat design, clean geometric lines, professional brand mark
```

示例（时尚品牌）：
```
A minimalist fashion logo formed by only sunglasses and lips, 
reduced to absolute minimum, bare minimum representation, 
solid black on pure white background, vector flat design, 
clean lines, professional brand identity
```

### 2. 负空间双关

```
A clever negative space logo: [主体A] silhouette where the empty 
space inside forms [主体B], dual meaning figure-ground design, 
both images clearly readable, solid black on pure white background, 
vector flat, minimalist, professional brand mark
```

示例（茉莉奶白风格）：
```
A clever negative space logo: eight-petal jasmine flower silhouette 
where the center empty space forms a Chinese character "白", 
dual meaning figure-ground design, both clearly readable, 
solid white on pure black background, vector flat, minimalist
```

### 3. 实物切入点

```
A logo derived from the silhouette of [实物], geometrically 
abstracted, smooth simplified outline, only outer contour with 
no internal details, [颜色] on [背景色] background, vector flat, 
minimalist, clean professional brand identity
```

示例（母婴品牌）：
```
A logo derived from the silhouette of a baby foot, geometrically 
abstracted, smooth simplified outline, only outer contour, 
solid black on pure white background, vector flat, minimalist
```

### 4. 字母共笔

```
A monogram logo of letters [字母1] and [字母2] sharing a common 
stroke, intertwined as one inseparable form, elegant serif-inspired 
curves, both letters individually recognizable, solid [颜色] on 
pure [背景色] background, vector flat, luxury brand identity, 
minimalist
```

示例（S+J）：
```
A monogram logo of letters S and J sharing a common curved stroke, 
intertwined as one elegant S-shaped form, both letters individually 
recognizable, solid black on pure white background, vector flat, 
luxury fashion brand identity, minimalist
```

### 5. 图形同构

```
A creative logo merging [意象A] and [意象B] where their similar 
curves fuse into one shape, isomorphic dual-image, both forms 
simultaneously visible, solid [颜色] on pure [背景色] background, 
vector flat, minimalist, clever brand mark
```

示例（鸟+音乐）：
```
A creative logo merging a flying bird and musical notes where 
their similar curves fuse into one shape, the bird's wing gaps 
forming notes, isomorphic dual-image, solid blue on pure white 
background, vector flat, minimalist
```

### 6. 圆切手法

```
A geometric logo constructed from intersecting circles, [数量] 
petal/leaf shapes formed by circle intersections, mathematically 
precise organic curves, all arcs from perfect circles, solid 
[颜色] on pure [背景色] background, vector flat, minimalist, 
golden ratio proportions
```

示例（茉莉花）：
```
A geometric jasmine flower logo constructed from 8 intersecting 
circles, 8 petals formed by circle intersections, mathematically 
precise organic curves, solid white on pure black background, 
vector flat, minimalist
```

### 7. 描边轮廓

```
A [主体] logo in monoline outline style, single uniform stroke 
weight, clean closed contour, no fill, [颜色] line on pure 
[背景色] background, vector flat, minimalist, modern icon style
```

示例（星星）：
```
A star logo in monoline outline style, single uniform stroke 
weight, clean closed contour, no fill, black line on pure white 
background, vector flat, minimalist
```

### 8. 字母意象化

```
A conceptual logo of letter [字母] where [具体笔画] transforms 
into [意象], the letter remains recognizable, natural integration, 
solid [颜色] on pure [背景色] background, vector flat, 
minimalist, dynamic brand identity
```

示例（O+流星）：
```
A conceptual logo of letter O where a shooting star streaks 
across the ring, the O remains recognizable as a circle, natural 
integration of star trail, solid black on pure white background, 
vector flat, minimalist
```

### 9. 替换笔画

```
A wordmark logo of [文字] where the [笔画描述] is replaced by 
a [图形], the text remains fully readable, graphic matches stroke 
weight, solid [颜色] on pure [背景色] background, vector flat, 
custom lettering, minimalist
```

### 10. 留白+传统图样

```
A modern oriental logo: [传统图样] simplified to minimal form, 
large areas of negative space, only 1-2 key traditional elements 
retained, [颜色] on pure [背景色] background, vector flat, 
contemporary chinese aesthetic, minimalist
```

## 配色方案

根据品牌调性选择：
- **高端/奢侈**：`solid black on pure white` 或 `solid white on pure black`
- **科技/互联网**：`solid deep blue (#1a1a2e) on pure white`
- **餐饮/食品**：`solid warm orange on pure white`
- **自然/有机**：`solid forest green on pure white`
- **女性/美妆**：`solid rose pink on pure white`
- **文化/新中式**：`solid vermillion red on pure white` 或 `solid gold on pure black`

## 尺寸建议

- 默认 2048x2048（1:1 正方形，适合logo展示）
- 如需横版展示：2048x1152（16:9）
- 如需竖版：1152x2048（9:16）

## 生成后检查

生成图片后必须检查：
1. 图形是否清晰、无多余元素
2. 是否意外生成了文字（AI常误生成，如有则重新生成）
3. 负空间/双关是否可读
4. 背景是否纯净
5. 如不满意，调整prompt中的描述词重新生成，最多3次
