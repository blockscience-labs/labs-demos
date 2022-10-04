# Presenting your Work
<blockquote>There is no cost to getting things wrong. The cost is not getting
them published. - Brian Nosek</blockquote>

BlockScience Labs provides a number of publishing features and services to get your hard work into the hands of stakeholders or other interested parties that only want to see the end results.

<iframe width="560" height="315" src="https://www.youtube.com/embed/ZVucoTOTx00" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Docsite Publishing
One of our key features for presenting work is through a static website generated from markdown files. We generally refer to this website as a *docsite* or *documentation site* and creating one for you project is super simple.

### mkdocs
To generate your projects docsite, you simply need to add a `docs/` folder in the root of your Git repo and populate it with markdown files. Since we use [mkdocs](https://mkdocs.org) to generate these sites, you can simply refer to their own documentation for usage details. We will generate a configuration file for you if one is not supplied but feel free to add one to really customize your docsite presentation and behavior.

!!!info
    Only three themes are installed and able to be used at the moment: `material` (default), `readthedocs`, and `mkdocs`. The `material` theme uses a color scheme provided by the Labs platform but you can override that using the normal methods detailed [here](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/).
    
!!!info
    MathJax/LaTeX is enabled by default so you don't need to do anything additional to get this working.

## Document Hosting
From within the JupyterLab IDE, you can publish + host static version of `markdown` and `notebook` files by right clicking on those types of files and selecting `Publish Document` from the contextual menu. Any other file can be hosted by right clicking and selecting `Host Document`. Both scenarios will present you with the option to select whether or not you want the file to be published/hosted publicly or privately.

<iframe width="560" height="315" src="https://www.youtube.com/embed/QOdy1yboOMs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>