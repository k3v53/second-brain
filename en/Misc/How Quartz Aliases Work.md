---
title: 
aliases: 
tags:
  - English
  - Quartz-4
draft: false
status: PseudoFinished
---
The plugin [AliasRedirects](https://quartz.jzhao.xyz/plugins/AliasRedirects) takes the aliases of the pages and treats them relatively to the place where the note is stored and then, it places them as an absolute path from the website you've specified in the config file. an example below

> [!example] 
> my page is located in `folder/subfolder/page` and has the alias `../old_subfolder/page`, the resulting url redirection is:
> `https://mysite.com/folder/old_subfolder/page` > `https://mysite.com/folder/subfolder/page` 
> Because my new subfolder is in the same folder as the old subfolder.
> 
> Folder Structure:
> - folder
> 	- subfolder
> 		- page
> 	- old_subfolder

If you are doing this and the redirection doesn't work, keep in mind that the aliases should be written with dashes (`-`) instead of spaces for it to work.
> [!Example]
> ✅ Good: `../folder/my-crazy-long-note`
> 🚫 Bad:   `../folder/my crazy long note`

> [!info]
> Keep in mind that the aliases are case-sensitive.
# Sources
- [A comment that I've auto responded to myself](https://github.com/jackyzha0/quartz/issues/904#issuecomment-2327612824)
- https://quartz.jzhao.xyz/plugins/AliasRedirects