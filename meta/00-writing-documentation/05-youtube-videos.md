# YouTube Videos
Display YouTube videos directly in documentation.

# Motivation

Markdown does not have a way to directly embed webpages or videos. Since videos will be a big part of Wise Software's knowledge base, you will be able to embed YouTube videos.

# Using YouTube Videos

Every YouTube video has a link containing an ID. The id is the part after the `?v=` on its URL. For example, the ID of the video at `https://www.youtube.com/watch?v=dQw4w9WgXcQ` is `dQw4w9WgXcQ`.

Once you have the ID, embed it using the Youtube component: `@youtube[id]`. For the video above, you would use `@youtube[dQw4w9WgXcQ]`.

Make sure that the video is on its own line! It should look like this:
```md
Paragraph.

@youtube[dQw4w9WgXcQ]

Other paragraph.
```

## Example

@youtube[dQw4w9WgXcQ]


# YouTube Spec

```md
@youtube[String id]
```
## Primary

```md
@youtube[String id]
```

Embed a YouTube video.

| Parameter | Type   | Description                           |
| --------- | ------ | ------------------------------------- |
| id        | String | The ID of the YouTube video to embed. |
