---
title: Topological approaches to understanding multi-human team EEG state
subtitle: Abstract 👋 33rd Annual Computational Neuroscience Meeting CNS*2024, Natal, Brazil

# Summary for listings and search engines
summary: Abstract 👋 How can we capture structure in high-dimensional behavioral and physiological data obtained from human subjects performing a teaming task? For example, EEG data is often collected across n bands at a high sampling rate. This results in large quantities of data points that live in n-dimensional (n-dim) space. One approach is use topological data analysis to identify and study the underlying structure of data. Topology is a field of mathematics concerned with the shape and connectivity of spaces. Mapper is a topological tool that allows the user investigate a dataset's connectivity [1]. The Mapper algorithm takes in high-dimensional data, projects it down to lower dimensional space, groups it there, and then applies those groupings to the original data points, where it connects clusters whenever two clusters contain a point, see (Fig. 1 -- top). Mapper allows for observation of underlying patterns and structure that are impossible to visualize or understand in the original space.

Mapper has been used previously by Saggar et. al, for example see [2], to analyze MRI data collected from five different tasks, instructions, working memory, video, math, and rest. The authors showed that Mapper could elucidate the relationship between behavior and the evolution of underlying brain states over time and across tasks and represent it in a hub-like network. Building on this work, we use Mapper to provide insight into a multi-human finger tapping teaming task that includes both behavioral and EEG data. Applying Mapper to understand properties from EEG time-series data as opposed to MRI data will require overcoming signal noise, artifacts, and the signal's non-linear nature.

We present results from data collected from a set of collaborative tapping tasks. Participants were paired off, isolated, and instructed to tap synchronously or syncopated to a metronome's beat. Next, subjects had to self-pace, pace off of their partner, lead their partner, or pace off of each other, depending on the trial. We analyzed EEG data across 32 different channels at a sample rate of 2000Hz, which yielded datasets consisting of ~800,000 data points in 32-dim space for each of the 12 trials. For each dataset, we fed the 32-dim data into Mapper where it projected it down to 2-dim using t-SNE. There, Mapper grouped the points in the 2-dim space and applied those groupings to the points in the 32-dim space. Finally, Mapper clustered the groups using DBSCAN and built a graph where clusters that contained the same points were connected, see (Fig. 1 -- bottom).

We observed structural differences between the Mapper graphs of the two tapper's brain states across all 12 tasks. Across time, one individual showed distinct partitioning between the self-led task and the other three tasks. Finally, the graphs exhibited hub-like behavior, similar to those referenced above by Sagger et. al [2].

# Link this post with a project
projects: []

# Date published
date: '2024-7-13T00:00:00Z'

# Date updated
lastmod: '2024-7-13T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/CpkOjOcXdUY)'
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - Brittany Story
  - Zhibin Zhou
  - Ramesh Srinivasan
  - Javier Omar Garcia
  - Piotr Franaszczuk
  - David Boothe

tags:
  - Academic
  - 开源

categories:
  - Demo
  - 教程
---

```python
import libr
print('hello')
```

## Abstract

1. How can we capture structure in high-dimensional behavioral and physiological data obtained from human subjects performing a teaming task? For example, EEG data is often collected across n bands at a high sampling rate. This results in large quantities of data points that live in n-dimensional (n-dim) space. One approach is use topological data analysis to identify and study the underlying structure of data. Topology is a field of mathematics concerned with the shape and connectivity of spaces. Mapper is a topological tool that allows the user investigate a dataset's connectivity [1]. The Mapper algorithm takes in high-dimensional data, projects it down to lower dimensional space, groups it there, and then applies those groupings to the original data points, where it connects clusters whenever two clusters contain a point, see (Fig. 1 -- top). Mapper allows for observation of underlying patterns and structure that are impossible to visualize or understand in the original space.
2. Mapper has been used previously by Saggar et. al, for example see [2], to analyze MRI data collected from five different tasks, instructions, working memory, video, math, and rest. The authors showed that Mapper could elucidate the relationship between behavior and the evolution of underlying brain states over time and across tasks and represent it in a hub-like network. Building on this work, we use Mapper to provide insight into a multi-human finger tapping teaming task that includes both behavioral and EEG data. Applying Mapper to understand properties from EEG time-series data as opposed to MRI data will require overcoming signal noise, artifacts, and the signal's non-linear nature.
**no-code solution (write in Markdown and customize with YAML parameters)** and having **flexibility to later add even deeper personalization with HTML and CSS**
3. We present results from data collected from a set of collaborative tapping tasks. Participants were paired off, isolated, and instructed to tap synchronously or syncopated to a metronome's beat. Next, subjects had to self-pace, pace off of their partner, lead their partner, or pace off of each other, depending on the trial. We analyzed EEG data across 32 different channels at a sample rate of 2000Hz, which yielded datasets consisting of ~800,000 data points in 32-dim space for each of the 12 trials. For each dataset, we fed the 32-dim data into Mapper where it projected it down to 2-dim using t-SNE. There, Mapper grouped the points in the 2-dim space and applied those groupings to the points in the 32-dim space. Finally, Mapper clustered the groups using DBSCAN and built a graph where clusters that contained the same points were connected, see (Fig. 1 -- bottom).

[![We observed structural differences between the Mapper graphs of the two tapper's brain states across all 12 tasks. Across time, one individual showed distinct partitioning between the self-led task and the other three tasks. Finally, the graphs exhibited hub-like behavior, similar to those referenced above by Sagger et. al [2].](https://raw.githubusercontent.com/wowchemy/wowchemy-hugo-modules/main/starters/academic/preview.png)](https://hugoblox.com)

## Get Started

- 👉 [**Create a new site**](https://hugoblox.com/templates/)
- 📚 [**Personalize your site**](https://docs.hugoblox.com/)
- 💬 [Chat with the **Wowchemy community**](https://discord.gg/z8wNYzb) or [**Hugo community**](https://discourse.gohugo.io)
- 🐦 Twitter: [@wowchemy](https://twitter.com/wowchemy) [@GeorgeCushen](https://twitter.com/GeorgeCushen) [#MadeWithWowchemy](https://twitter.com/search?q=%23MadeWithWowchemy&src=typed_query)
- 💡 [Request a **feature** or report a **bug** for _Wowchemy_](https://github.com/HugoBlox/hugo-blox-builder/issues)
- ⬆️ **Updating Wowchemy?** View the [Update Tutorial](https://docs.hugoblox.com/hugo-tutorials/update/) and [Release Notes](https://hugoblox.com/updates/)

## Acknowledgements
We thank the US Army Research Lab for funding Ramesh Srinivasan and Zhibin Zhou under Contract No W911NF2420013.
References:

[1] Singh, G., Mémoli, F., & Carlsson, G. (2007). Topological Methods for the Analysis of High Dimensional Data Sets and 3D Object Recognition. Eurographics Symposium on Point-Based Graphics 2007, 91-100. 
[2] Saggar, M., Sporns, O., Gonzalez-Castillo, J., et al. (2018). Towards a new approach to reveal dynamical organization of the brain using topological data analysis. Nature Communications, 9, 1399. 

### [❤️ Click here to become a sponsor and help support Wowchemy's future ❤️](https://hugoblox.com/sponsor/)

As a token of appreciation for sponsoring, you can **unlock [these](https://hugoblox.com/sponsor/) awesome rewards and extra features 🦄✨**

## Ecosystem

- **[Hugo Academic CLI](https://github.com/GetRD/academic-file-converter):** Automatically import publications from BibTeX

## Inspiration

[Check out the latest **demo**](https://academic-demo.netlify.com/) of what you'll get in less than 10 minutes, or [view the **showcase**](https://hugoblox.com/user-stories/) of personal, project, and business sites.

## Features

- **Page builder** - Create _anything_ with [**widgets**](https://docs.hugoblox.com/page-builder/) and [**elements**](https://docs.hugoblox.com/content/writing-markdown-latex/)
- **Edit any type of content** - Blog posts, publications, talks, slides, projects, and more!
- **Create content** in [**Markdown**](https://docs.hugoblox.com/content/writing-markdown-latex/), [**Jupyter**](https://docs.hugoblox.com/import/jupyter/), or [**RStudio**](https://docs.hugoblox.com/install-locally/)
- **Plugin System** - Fully customizable [**color** and **font themes**](https://docs.hugoblox.com/customization/)
- **Display Code and Math** - Code highlighting and [LaTeX math](https://en.wikibooks.org/wiki/LaTeX/Mathematics) supported
- **Integrations** - [Google Analytics](https://analytics.google.com), [Disqus commenting](https://disqus.com), Maps, Contact Forms, and more!
- **Beautiful Site** - Simple and refreshing one page design
- **Industry-Leading SEO** - Help get your website found on search engines and social media
- **Media Galleries** - Display your images and videos with captions in a customizable gallery
- **Mobile Friendly** - Look amazing on every screen with a mobile friendly version of your site
- **Multi-language** - 34+ language packs including English, 中文, and Português
- **Multi-user** - Each author gets their own profile page
- **Privacy Pack** - Assists with GDPR
- **Stand Out** - Bring your site to life with animation, parallax backgrounds, and scroll effects
- **One-Click Deployment** - No servers. No databases. Only files.

## Themes

Wowchemy and its templates come with **automatic day (light) and night (dark) mode** built-in. Alternatively, visitors can choose their preferred mode - click the moon icon in the top right of the [Demo](https://academic-demo.netlify.com/) to see it in action! Day/night mode can also be disabled by the site admin in `params.toml`.

[Choose a stunning **theme** and **font**](https://docs.hugoblox.com/customization) for your site. Themes are fully customizable.

## License

Copyright 2016-present [George Cushen](https://georgecushen.com).

Released under the [MIT](https://github.com/HugoBlox/hugo-blox-builder/blob/master/LICENSE.md) license.
