# 22_mdx-svg
[../22_mdx-svg](../22_mdx-svg)

Example for testing SVG usage within `.astro`, `.md` and `.mdx`

This highlights incompatibility of inlined SVG when injected from remark/rehype plugins in an mdx file
* attributes with ':' e.g. `xmlns:xlink` gets treated as .jsx and converted to `xmlnsXlink`, `xmlns` or `xmlnsxlink`, all of which break the SVG rendering

Note :
* html comments not supported
* html empty new lines of spaces also break the html parsing as indentation takes precendence

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/MicroWebStacks/astro-examples/tree/main/22_mdx-svg)
[![open in Codesandbox](../media/codesandbox.svg)](https://codesandbox.io/s/github/MicroWebStacks/astro-examples/tree/main/22_mdx-svg)
[![open in Gitpod](../media/gitpod.svg)](https://gitpod.io/?on=gitpod#https://github.com/MicroWebStacks/astro-examples/tree/main/22_mdx-svg)

[![Open in Codeanywhere](https://codeanywhere.com/img/open-in-codeanywhere-btn.svg)](https://app.codeanywhere.com/#https://github.com/MicroWebStacks/astro-examples)

## references
* github issue https://github.com/withastro/astro/issues/5796#issuecomment-1374766914
* Stackoverflow https://stackoverflow.com/questions/73306060/title-is-undefined-while-generating-sitemap-in-astro
* Stackoverflow https://stackoverflow.com/questions/75119497/how-can-i-filter-frontmatter-in-a-remark-plugin
