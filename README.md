# DesignWrap Shopify Product Image Studio

[中文](#中文说明) · [English](#english)

An AI skill by [DesignWrap](https://designwrap.co) that turns uploaded product photos into consistent, clean Shopify catalogue images.

## 中文说明

### 这是什么？

**DesignWrap Shopify Product Image Studio** 是一个用于 ChatGPT / Codex 的 Shopify 产品图片处理 Skill。

你可以将产品原图交给它处理。它会先检查每张图片是否适合转换，再以统一的白底、电商目录风格逐张输出，同时锁定产品本身的轮廓、颜色、材质与细节。

它的目标不是重新设计产品，而是减少为 Shopify 商品图手动抠图、统一背景和调整画布的重复工作，让产品图片在店铺网格中保持专业、整齐且一致。

### 它可以做什么？

- 将适合处理的产品图片转换为纯白（`#FFFFFF`）无缝背景
- 在产品正下方保留轻微、自然的浅灰色接触阴影
- 默认输出 `2048 × 2048 px` 的 1:1 高清 WebP 产品图
- 让整批产品保持居中、直立、完整不裁切，并拥有一致的视觉比例
- 为不同颜色、款式或拍摄角度分别生成图片，不会混合成同一张图
- 保留产品原有的轮廓、颜色、材质、纹理、车线、Logo、标签、五金与印刷文字
- 识别不适合直接转换的图片，并说明需要确认的原因
- 不覆盖原始文件，并使用清晰稳定的文件命名方式

### 它不会做什么？

- 不会重新设计、补全、移除、重绘或虚构产品细节
- 不会改变产品颜色、比例、材质、Logo、标签、印刷文字或五金
- 不会擅自将生活方式图片变成抠图产品图
- 不会未经确认移除图片中的人物、宠物或复杂场景主体
- 不会将多个独立产品合并到同一张图片中
- 不会生成水印、边框、文字、相框、色偏、额外道具或生硬阴影

如果产品拍摄于人物、宠物或复杂场景中，而移除主体可能改变产品展示方式，Skill 会先询问你的处理方向。

### 适合谁？

- 需要统一 Shopify 商品图库视觉的品牌与商家
- 有一批产品原图需要快速处理为白底图的店主
- 希望减少抠图和画布整理工作，但不想牺牲产品真实性的电商团队
- 为客户准备 Shopify 商品目录的设计师、摄影师与开发者

### 安装方式

1. 下载或克隆这个仓库。
2. 将 `designwrap-shopify-product-image-studio` 文件夹添加到支持 Skills 的 ChatGPT / Codex 环境。
3. 上传产品图片，然后调用 `@DesignWrap Shopify Product Image Studio`。

不同版本的 ChatGPT / Codex 安装入口可能不同，请以你当前产品界面为准。

### 示例指令

```text
@DesignWrap Shopify Product Image Studio 请将我上传的所有产品图片处理为 Shopify 产品图：
纯白背景、产品下方轻微自然投影、1:1、2048 × 2048 px 高清 WebP。
请保留产品的原始颜色、Logo、材质、细节和比例；不要裁切或改变产品本身。
```

### 工作流程

1. 识别本次上传的全部产品图片，并将每张图片作为独立输出处理。
2. 检查每张图片，判断它是否是简单产品图、带人物/场景的图片，或是不宜安全转换的图片。
3. 为符合条件的图片创建白底电商产品图，锁定产品的真实形状与细节。
4. 保持产品居中、直立、不裁切，并让同批图片有一致的视觉比例。
5. 检查背景是否为纯白、边缘是否自然、投影是否柔和，以及产品是否出现任何偏差。
6. 返回完成图片，并说明被排除或需要进一步确认的图片及原因。

### 关于 DesignWrap

[DesignWrap](https://designwrap.co) 是一家位于澳大利亚墨尔本的独立数字设计工作室，专注于 Shopify、Webflow 和 Framer 网站设计与开发。这个 Skill 来自真实的 Shopify 客户项目流程，用来减少重复的产品图片处理工作，让品牌和设计团队把时间放在更重要的产品、内容和客户体验上。

如果你需要定制 Shopify 网站、产品详情页规划或电商视觉系统设计，可以联系 DesignWrap。

---

## English

### What is it?

**DesignWrap Shopify Product Image Studio** is a Shopify product-image preparation skill for ChatGPT / Codex.

Give it your source product photos. It first checks whether each image is suitable for conversion, then produces a consistent white-background ecommerce image for every qualifying photo while keeping the product's shape, colour, materials, and details intact.

The goal is not to redesign the product. It is to reduce repetitive background cleanup and canvas preparation for Shopify while keeping a product grid polished, consistent, and truthful to the original item.

### What can it do?

- Convert suitable product photos to a seamless pure-white (`#FFFFFF`) background
- Add one subtle, natural light-grey contact shadow directly beneath the product
- Produce 1:1, 2048 × 2048 px high-resolution WebP images by default
- Keep a batch centred, upright, uncropped, and visually consistent in scale
- Create separate images for distinct colours, styles, and product angles
- Preserve the original silhouette, colour, material, texture, seams, logos, labels, hardware, and printed copy
- Flag images that cannot be safely converted and explain what needs direction
- Keep original files intact and use clear, stable output names

### What will it not do?

- It will not redesign, fill in, remove, redraw, or invent product details
- It will not alter product colour, proportions, materials, logos, labels, printed copy, or hardware
- It will not silently turn lifestyle photography into a product cutout
- It will not remove people, pets, or complex scenes without confirmation
- It will not merge independent products into one image
- It will not add watermarks, borders, text, frames, colour casts, props, or harsh shadows

When a product is photographed on a person, pet, or complex scene, and removing the subject could change the product presentation, the skill asks for direction first.

### Who is it for?

- Brands and merchants building a consistent Shopify product gallery
- Store owners preparing a batch of source photos as white-background product images
- Ecommerce teams that want less manual cleanup without compromising product accuracy
- Designers, photographers, and developers preparing catalogues for Shopify clients

### Installation

1. Download or clone this repository.
2. Add the `designwrap-shopify-product-image-studio` folder to a ChatGPT / Codex environment that supports Skills.
3. Upload your product photos, then invoke `@DesignWrap Shopify Product Image Studio`.

The exact installation entry point may differ between ChatGPT / Codex versions. Follow the interface available in your product.

### Example prompt

```text
@DesignWrap Shopify Product Image Studio, convert all product photos I uploaded into Shopify product images:
pure white background, a subtle natural contact shadow, 1:1, 2048 × 2048 px high-resolution WebP.
Preserve the product's original colour, logos, materials, details, and proportions. Do not crop or alter the product itself.
```

### How it works

1. Identify every uploaded product photo and treat each one as a separate output.
2. Inspect each image to determine whether it is a simple product photo, an image with a person or scene, or unsafe to transform without direction.
3. Create a white-background ecommerce image for qualifying photos while locking the product's real shape and details.
4. Keep products centred, upright, uncropped, and visually consistent across the batch.
5. Check that the background is pure white, edges are natural, shadows are restrained, and the product has not drifted.
6. Return the finished images and explain any excluded images or images that need direction.

### About DesignWrap

[DesignWrap](https://designwrap.co) is an independent digital design studio based in Melbourne, Australia, specializing in Shopify, Webflow, and Framer design and development. This skill comes from a real Shopify client-delivery workflow. It was created to reduce repetitive product-image preparation so brands and design teams can focus on product, content, and customer experience.

For custom Shopify design, PDP planning, or ecommerce visual-system design, contact DesignWrap.

## Repository structure

```text
designwrap-shopify-product-image-studio/
├── SKILL.md
├── README.md
└── agents/
    └── openai.yaml
```

## Disclaimer

This is an independent project by DesignWrap. It is not affiliated with or endorsed by Shopify or OpenAI. Shopify, ChatGPT, and Codex are trademarks of their respective owners.
