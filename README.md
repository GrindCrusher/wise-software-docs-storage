# Documentation
The source for Wise Software's documentation. Only members in the Documentation team may edit. Please request access if you are not in it.

## `structure.yml`
This file contains the metadata for all environments (in a sense, a collection of categories and pages for a specific product). A typical environment will look like this:

```yml
- displayName: Environment Name
  description: A description of this environment.
  displayIcon: https://cdn.realsgii2.dev/wise-software-docs-static/wiseMobile.png
  color: "#ff0000"
```

Structures are shown on the main page:

![image](https://github.com/wise-software-inc/documentation/assets/41650610/369c6f97-c167-4cd9-a8e6-176100f7fbd0)

And on the Environment Picker: 

![image](https://github.com/wise-software-inc/documentation/assets/41650610/9942511a-a35c-4b0b-bd94-f4ad5d97e887)

## Markdown
Pages for the documentation are written in [GFM](https://github.github.com/gfm/) (GitHub Flavored Markdown).

### Custom Components
There are a few custom components to aid in successful documentation

#### YouTube Embeds
You may embed a YouTube video using `@youtube[videoId]`. For example, [https://www.youtube.com/watch?v=dQw4w9WgXcQ](https://www.youtube.com/watch?v=dQw4w9WgXcQ) will be embeded as `@youtube[dQw4w9WgXcQ]`.

#### Image Grids
You may align two or more images side-by-side. To do this, use the following format:
```md
@image-grid
![image1](https://github.com/wise-software-inc/documentation/assets/41650610/369c6f97-c167-4cd9-a8e6-176100f7fbd0)
![image2](https://github.com/wise-software-inc/documentation/assets/41650610/9942511a-a35c-4b0b-bd94-f4ad5d97e887)
```

Be sure to NOT include any additional line breaks, as those will close the grid. **Below is an example of an invalid image grid.**
```md
@image-grid

![image1](https://github.com/wise-software-inc/documentation/assets/41650610/369c6f97-c167-4cd9-a8e6-176100f7fbd0)

![image2](https://github.com/wise-software-inc/documentation/assets/41650610/9942511a-a35c-4b0b-bd94-f4ad5d97e887)
```

This will look just as if the image grid tag isn't there.
