---
title: Module Tags
taxonomy:
    category: docs
---

Reel 1.2 introduced module tags for searching YouTube and Vimeo. Below are examples of each tag with all the available variables. Queries to each service will be cached for quicker load times and to avoid repeated hits to each API.

The following parameters are available to both tags:

## ```query=”“```

> Optional. Enter any search string to use for querying videos.

## ```user=”“```

> Optional. Username to restrict all searches to. If no query parameter is used, defining a user will limit all video results to that user.

## ```limit=”“```

> Optional. Number of videos to show. Defaults to 20.

## ```offset=”“```

> Optional. Offset the query results. For example, do not show the first 3 videos.

## ```variable_prefix=”“```

> Optional. Allows you to prefix all variables within the tag to avoid possible collisions with other modules.

## ```width=”“```

> Optional. The width of the video if using the {embed} tag. Defaults to 360.

## ```height=”“```

> Optional. The height of the video if using the {embed} tag. Defaults to 240.

Tag examples with all available variables.

```
{exp:wyvern_video:youtube}
    {video_id}
    {title}
    {content} or {description}
    {url}
    {url_mobile}
    {thumbnail_0} {thumbnail_1} {thumbnail_2} {thumbnail_3}
    {author}
    {category}
    {keywords}
        {keyword}
    {/keywords}
    {duration}
    {view_count}
    {favorite_count}
    {id}
    {published}
    {updated}
    {embed}
{/exp:wyvern_video:youtube}
```

```
{exp:wyvern_video:vimeo}
    {video_id}
    {title}
    {content} or {description}
    {url}
    {url_mobile}
    {thumbnail_0} {thumbnail_1} {thumbnail_2} {thumbnail_3}
    {author}
    {tags}
        {tag}
    {/tags}
    {duration}
    {view_count}
    {favorite_count}
    {id}
    {published}
    {updated}
    {embed}
{/exp:wyvern_video:vimeo}
```