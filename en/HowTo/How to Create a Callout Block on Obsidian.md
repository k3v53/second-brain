---
tags:
  - English
  - Obsidian
  - Syntax
aliases:
  - Callout Block on Obsidian
status: Writing
---

> [!info]
> Hello World!
>```md
>> [!info]
>> Hello World!
> ```

> [!info] Custom Title
> Hello World With Custom Title!
>```md
>> [!info] Custom Title
>> Hello World With Custom Title!
> ```

> [!info]- Collapsible 
> Hello World!
>```md
>> [!info]- Collapsible
>> Hello World!
> ```

## Customize callouts

[CSS snippets](https://help.obsidian.md/Extending+Obsidian/CSS+snippets) and [Community plugins](https://help.obsidian.md/Extending+Obsidian/Community+plugins) can define custom callouts, or even overwrite the default configuration.

To define a custom callout, create the following CSS block:

```css
.callout[data-callout="custom-question-type"] {
    --callout-color: 0, 0, 0;
    --callout-icon: lucide-alert-circle;
}
```

The value of the `data-callout` attribute is the type identifier you want to use, for example `[!custom-question-type]`.

- `--callout-color` defines the background color using numbers (0–255) for red, green, and blue.
- `--callout-icon` can be an icon ID from [lucide.dev](https://lucide.dev), or an SVG element.
# Source
- https://help.obsidian.md/Editing+and+formatting/Callouts