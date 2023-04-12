---
{"dg-publish":true,"permalink":"/系统/👻 测试/Features/","noteIcon":"1","created":"2023-04-12T21:52:28.005+08:00","updated":""}
---

# Features

日期:: 2023-04-12T21:53:29 (UTC +08:00)
标签:: #参 []
来源:: https://dg-docs.ole.dev/features/
作者:: 

You can enable the following features in your digital garden, in the [note settings](https://dg-docs.ole.dev/getting-started/03-note-settings/):

-   Local Graph
-   Global Graph
-   Backlinks
-   Table Of Content
-   Filetree navigation
-   Link preview
-   Search
-   Frontmatter tags

Additionally the garden supports a variety of formatting and content types in your notes.

___

## Wikilinks

Link as you normally would in Obisidan, with the `[[Wikilink]]` syntax

Linking to a specific header works the same way as in Obsidian  
`[[My Note#Note header]]`

### Block links

Linking to a specific block works the same way as in Obsidian  
`[[My Note#^123abc]]`

### Custom link names

Changing display text for a wikilink works the same way as in Obsidian  
![CleanShot 2023-01-10 at 18.07.56@2x.png|250](https://dg-docs.ole.dev/img/user/img/CleanShot%202023-01-10%20at%2018.07.56@2x.png)

___

## Code Blocks

![CleanShot 2022-11-13 at 15.34.22@2x.png](https://dg-docs.ole.dev/img/user/img/CleanShot%202022-11-13%20at%2015.34.22@2x.png)

```
let a = 5;
```

![CleanShot 2022-11-13 at 15.34.59@2x.png|200](https://dg-docs.ole.dev/img/user/img/CleanShot%202022-11-13%20at%2015.34.59@2x.png)  
`Some inline code`

___

## Dataview queries

```
list from "Advanced"
```

-   [CSS Customization](https://dg-docs.ole.dev/advanced/css-customization/)
-   [Adding custom components](https://dg-docs.ole.dev/advanced/adding-custom-components/)
-   [Content Customization](https://dg-docs.ole.dev/advanced/content-customization/)
-   [Comparison to other solutions](https://dg-docs.ole.dev/advanced/comparison-to-other-solutions/)
-   [Configure build pipeline](https://dg-docs.ole.dev/advanced/configure-build-pipeline/)
-   [Dataview queries](https://dg-docs.ole.dev/advanced/dataview-queries/)
-   [Note Specific Settings](https://dg-docs.ole.dev/advanced/note-specific-settings/)
-   [Hosting alternatives](https://dg-docs.ole.dev/advanced/hosting-alternatives/)
-   [Adding comments](https://dg-docs.ole.dev/notes/advanced-guides-and-how-tos-adding-comments)
-   [Adding analytics](https://dg-docs.ole.dev/notes/advanced-guides-and-how-tos-adding-analytics)
-   [Fine grained access token](https://dg-docs.ole.dev/advanced/fine-grained-access-token/)
-   [Roadmap](https://dg-docs.ole.dev/advanced/roadmap/)
-   [Tips and Tricks](https://dg-docs.ole.dev/advanced/tips-and-tricks/)

More details about dataview is available here: [Dataview queries](https://dg-docs.ole.dev/advanced/dataview-queries/)

___

## Callouts

```
> [!NOTE] Note title
> Information
```

```
> [!WARNING] A warning
> This is a warning
```

### Folding Callouts

```
> [!NOTE]+ Open by default
> Folding/Collapsable callout
```

Folding/Collapsable callout

```
> [!FAQ]- Closed by default
> Folding/Collapsable callout
```

Folding/Collapsable callout

### Nested callouts

```
> [!TIP] Nested callouts
> Text inside the tip callout
> > [!EXAMPLE] Inner callout
> > Multiple nesting layers
> > > [!TODO] Inner inner callout
```

Text inside the tip callout

___

## MathJax / LaTex

[MathJax Reference](https://math.meta.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference)

```
$$\frac{1}{0} = \infty$$
```

10\=∞

___

Click on the tag below to view other pages with the same tag.

#exampletag

___

## Embedded/Transcluded Images

![CleanShot 2022-11-13 at 14.24.21@2x.png|250](https://dg-docs.ole.dev/img/user/img/CleanShot%202022-11-13%20at%2014.24.21@2x.png)

![obsidianlogo.png](https://dg-docs.ole.dev/img/user/img/obsidianlogo.png)

## Transcluded documents

### Whole file

![CleanShot 2022-11-13 at 14.24.50@2x.png|250](https://dg-docs.ole.dev/img/user/img/CleanShot%202022-11-13%20at%2014.24.50@2x.png)

[](https://dg-docs.ole.dev/example-pages/transcluded-document/)

This is a transcluded note.

This is a block in a transcluded document
{ #02502a}


Content

![CleanShot 2023-01-05 at 17.22.10.png](https://dg-docs.ole.dev/img/user/img/CleanShot%202023-01-05%20at%2017.22.10.png)

### Single Block

![CleanShot 2023-01-05 at 17.22.27.png](https://dg-docs.ole.dev/img/user/img/CleanShot%202023-01-05%20at%2017.22.27.png)

[](https://dg-docs.ole.dev/example-pages/transcluded-document/#02502a)

This is a block in a transcluded document

It's also worth noting that transclusions _do not need_ the dg-publish attribute. They behave the same as an image. If you transclude something into a document, and publish that document, everything that is transcluded in it will be published as if it was part of that note.

(More details on transclusion can be read here: [Content Customization#Tranclusions](https://dg-docs.ole.dev/advanced/content-customization/#tranclusions) )

___

## Excalidraw

![CleanShot 2022-11-13 at 14.25.34@2x.png|350](https://dg-docs.ole.dev/img/user/img/CleanShot%202022-11-13%20at%2014.25.34@2x.png)

Obsidian specific features like linking to other notes inside the drawings are currently not supported

___

## Mermaid diagrams

![CleanShot 2022-11-13 at 14.26.47@2x.png](https://dg-docs.ole.dev/img/user/img/CleanShot%202022-11-13%20at%2014.26.47@2x.png)

```
AB
```

![CleanShot 2022-11-13 at 14.27.14@2x.png](https://dg-docs.ole.dev/img/user/img/CleanShot%202022-11-13%20at%2014.27.14@2x.png)

```
A Gantt Diagram2014-01-052014-01-122014-01-192014-01-262014-02-022014-02-092014-02-16A task           Task in sec      another task     Another task     SectionAnotherA Gantt Diagram
```

___

## PlantUML diagrams

![uml diagram](https://www.plantuml.com/plantuml/svg/jLHTRzem57tthxWAhnjBCsWx52AwJdkRLAsR-a1vkCGtmIAn8zk8TjF--wuXq9HHrZqiaHBhVfvphks9ysZzggx4PB_oobS4jwRmQxIyU7IUQdWBrqPxL9gi4wAYmeCtO5Mvy22LfTmheuLmIwKRj5Z3Jm7W5YZDMkaI2gmSiGMjDUlFNEbM_I0uYzaagS1LvR_HWx-gLAbhqXvo_f1bxzfYSwUaNq0IX-WQ7xwGSrXIMo4MluHOA4d0E2qP_zXG5qU0XhgiA4rtdBQK-f_GunmTPTa6x4VCbwKrAoslJMKiz0RlBwKSiYVWRMt5vWdHnagohJMXy-H3Y6pJBQl4U1dP4uw6XJCwJRyxiYzrZ2y7oSNyDHtZOKB3ysSDNYPwH_EhfgbKZc58_vEksBA4Q3mEFEzrwdXAexCuczviFBFqNR1a4UoLG0TXnRcCYESAqS7UkzVJ0yiif3ydsR9wakDcMwq3_4XARx1vZYNkLJYH5YJOgHuuiz3GKRfBVtzwkWhyRKuipScGm_wx7VslZJiduS-MEsSORnWKzAUzYpYyR_n2vKlDnt6SpFhPQQmmWYZDWw2ZDZtZQYuIfxDUsso7yaYRhuJIGM5D3QWbtoZAa-FRAn8Jqd9p-Mt_lm40)

___

## Highlighted text

![CleanShot 2022-12-12 at 16.14.14@2x.png](https://dg-docs.ole.dev/img/user/img/CleanShot%202022-12-12%20at%2016.14.14@2x.png)

Here is some highlighted text

___

```
There is a footnote here [^1]
```

There is a footnote here <sup><a href="https://dg-docs.ole.dev/features/#fn1" id="fnref1">[1]</a></sup>

___

## Checkboxes

```
- [ ] Uncheckd
- [x] Checked
```

-   Uncheckd
-   Checked

___

## Sitemap

The site automatically generates a sitemap.xml file, available at `/sitemap.xml` on your site. This helps search engines properly index your site, making it more discoverable. For the sitemap to be properly formatted with the full URL for all your pages, the plugin needs to know the base URL of your site. By adding your URL to the plugin settings, the sitemap should automatically be generated using that value.

![CleanShot 2022-12-15 at 22.00.24@2x.png](https://dg-docs.ole.dev/img/user/img/CleanShot%202022-12-15%20at%2022.00.24@2x.png)

___

The site automatically generates an Atom/RSS feed available at `/feed.xml` on your site. In order for this to be generated you need to add your Base URL in the settings, like in the image above.  
For the dates to work properly, you need to enable the [Show updated timestamp](https://dg-docs.ole.dev/getting-started/04-appearance-settings/#timestamps-settings) setting under the plugin's Appearance settings. If this is not enabled, the feed will use the last date the site was built, which in practice means the last date you last published anything to the site.

___

```
[^1]: Here are some extra information in a footnote
```

___

1.  Here are some extra information in a footnote [↩︎](https://dg-docs.ole.dev/features/#fnref1)
