# Image Grid
Display mutliple images side by side.

# Motivation

Several images in a row creates longer pages, and adds to scrolling. This reduces user experience. Image grids fix this by displaying images side by side.

# Using Image Grids

Image grids are done in one block. Do not include blank lines between them, otherwise the grid will close unexpectedly. Here is an example: 

```
@img-grid
![img](https://i.wwise.dev/image-1.png)
![img](https://i.wwise.dev/image-2.png)
```

**Below is an invalid image grid and will not work. DO NOT USE!**
```
@img-grid

![img](https://i.wwise.dev/image-1.png)

![img](https://i.wwise.dev/image-2.png)
```

Do not include empty lines between the images or image grid tag.

# YouTube Spec

```md
@img-grid
{...}
```
## Primary

```md
@img-grid
{...}
```

Embed a partial.

| Parameter | Type     | Description                           |
| --------- | -------- | ------------------------------------- |
| ...       | Markdown | The content to include in the grid.   |
