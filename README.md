# Trustflows WebPoster for ISWC 2025

This repository contains the sources for a WebPoster of the poster paper titled: 

**Tackling the Write-to-Read Web of Data with Trustflows**
```
The need for the read–write Linked Data Web is currently implemented
as a Create, Read, Update or Delete (CRUD) strategy on resources
that implies that agents will read exactly what has once been written.
In practice, we notice the following problems when deploying writeable Linked Data nodes in an ecosystem.
Data reuse is impeded by diverging data usage requirements
from how the data was originally written and by evolving data models.
Also, individual data point verification at the read side becomes obligatory
due to the absence of an authoritative source that guarantees auditability.
We present characteristics of writeable Linked Data nodes (cope with longevity for written data,
combine read data using different models, and provide an explicit trust context)
as arguments justifying the need for a more complex operational model.
We apply a Command Query Responsibility Segregation pattern to decouple write and read interfaces,
introduce semantic mappings within the writeable Linked Data node to support evolving data read requirements,
and apply Event Sourcing aligned with PROV-O’s Actor-Entity-Activity model to provide an explicit trust context.
Applying this operational model – dubbed “Trustflows” – to the PACSOI use case
showcases the additional affordances of handling data coming in different granularities,
from different sources, adhering to different reading requirements.
```

Accepted for presentation at [ISWC 2025](https://iswc2025.semanticweb.org/#/program/acceptedpapers).

## How to build?

Clone thjis repository and follow the instructions below.

Install the dependencies and run the development server:

```bash
npm install
npm run dev
```

Edit `index.html` to customize your poster content.
- You can configure your theme colors and font in `css/style.scss`
- You can choose different section layouts by using the grid-column and grid-row CSS properties.
- You can add icons from [Font Awesome](https://fontawesome.com/icons) by adding the relevant classes to the `<i>` elements.
- You can add images by placing them in the `images` folder and referencing them in your HTML.

## How to deploy?

You can deploy your poster to GitHub Pages or any static site hosting service.

This repository already contains a configured GitHub Action that publishes the poster to GitHub Pages.

You can locally build and test the production version with:

```bash
npm run build
npm run preview
```
