---
name: designwrap-shopify-product-image-studio
description: Prepare uploaded product photos for Shopify by creating consistent, high-resolution white-background product images with a subtle natural shadow. Use for product-photo cleanup and catalog-ready image batches, not lifestyle or campaign imagery.
---

# DesignWrap Shopify Product Image Studio

Turn every uploaded image in scope into a consistent Shopify product image. Default to a clean, commercially neutral catalogue look:

- pure white (#FFFFFF) background;
- natural, very soft contact shadow below the product only;
- square 1:1 canvas, 2048 × 2048 px, suitable for a consistent Shopify product grid;
- sharp, high-resolution WebP output, without a watermark, border, text, frame, or colour cast.

## Workflow

1. Identify the image set and treat every uploaded product image as in scope unless the user narrows it. Keep colour variants and distinct angles as separate outputs.
2. Inspect each image first. Classify it as a simple product cutout, a product-on-model/lifestyle image, or an image that cannot safely be transformed without changing the product.
3. For each suitable image, use the built-in image generation editor in **edit** mode. Process images individually so the original product's shape, construction, texture, markings, logo, and colourway remain locked.
4. Output one finished image per source. Keep the product upright and centred, with visually consistent scale across the batch. Aim for about 70–85% of the canvas height while retaining comfortable white breathing room; do not crop any product edge.
5. Inspect each result before delivery. Redo only the affected image when the product has drifted, edges look artificial, the background is off-white, the shadow is too heavy, or the output is not square and crisp.

## Product-preservation rules

- Change the backdrop and presentation only. Do not redesign, invent, remove, recolour, smooth, or add product details.
- Preserve exact logos, printed copy, labels, hardware, material texture, seams, proportions, and product colour. Do not generate replacement text.
- Do not merge separate products into one frame. Treat bundles as one product only when they appear together in the original image.
- Keep intentional transparent, reflective, white, or pale product areas visibly distinct from the white background through accurate edges and a restrained contact shadow—not outlines.
- For products on a person, a pet, or a complex scene, ask whether the subject should also be removed. Do not silently turn a lifestyle image into a cutout when that would change the product presentation.

## Default edit specification

Use this concise specification for every qualifying image, adapting only the product description:

```text
Use case: background-extraction
Asset type: Shopify product gallery image
Primary request: Convert this into a clean e-commerce catalogue image.
Scene/backdrop: seamless pure white (#FFFFFF) studio background.
Subject: the exact product in the supplied image.
Composition/framing: centered, upright product on a square 1:1 canvas; retain all edges; product fills roughly 70–85% of canvas height.
Lighting/mood: even premium studio lighting with one subtle, diffuse, light-grey contact shadow directly beneath the product.
Constraints: change only the background and presentation. Preserve the product's exact silhouette, colour, material, seams, logos, labels, hardware, printed text, and proportions. High-detail crisp edges. No cropping.
Avoid: off-white or coloured background, hard or floating shadow, reflection, outline, extra objects, props, hands, people, pets, text changes, watermark, border, or invented details.
```

## Output choices

- Use the 1:1 2048 × 2048 px WebP default unless the user supplies an established Shopify image ratio, theme requirement, or a different desired size. Preserve that explicit requirement across the whole set.
- If the current Shopify store uses another consistent ratio (for example 4:5), match it rather than mixing ratios.
- Name files clearly in source order, using a stable product/colour/angle suffix when that information is available. Never overwrite the originals.
- State which image(s) were excluded or need user direction, and why.
