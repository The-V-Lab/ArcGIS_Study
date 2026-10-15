# ArcGIS Study | Getting Started with ArcGIS

A structured ArcGIS learning module for GIS beginners. It starts from spatial thinking, data models and coordinate systems, then covers ArcGIS Pro project management, cartography, queries and joins, basic geoprocessing, editing, layout and export, sharing in ArcGIS Online, reproducible workflows and responsible spatial practice.

## Course

| R Markdown source | Rendered HTML |
|---|---|
| [arcgis_getting_started_en.Rmd](./arcgis_getting_started_en.Rmd) | [arcgis_getting_started_en.html](./arcgis_getting_started_en.html) |

The HTML file is a self-contained page: clone or download the repository and open it directly in a browser. GitHub's ordinary file preview does not run HTML as a course website.

## Goals

The module does not teach ArcGIS as a set of buttons to memorize. It builds a spatial-analysis chain you can check, explain and repeat:

> **Ask a spatial question → check data and metadata → choose a coordinate system → explore and map → query, join and analyze → validate outputs → design the map → share safely**

By the end of the course, learners should be able to:

- explain the geometry, attributes, spatial reference and metadata of spatial data;
- distinguish projects, maps, layers, datasets, layouts, project items, web layers and web maps;
- recognize when points, lines, polygons, rasters and non-spatial tables are appropriate;
- create a project in ArcGIS Pro, connect data, inspect attributes and organize outputs;
- tell geographic from projected coordinate systems, and **Define Projection** from **Project**;
- choose symbols, colours, classifications, labels and pop-ups to suit the variable type;
- use attribute queries, spatial selections, attribute joins and spatial joins correctly;
- understand basic tools such as Buffer, Clip, Dissolve, Intersect, Spatial Join and Near;
- check record counts, fields, extents, units, geometry and edge cases;
- build layouts, export maps and share in ArcGIS Online for the intended audience;
- start building repeatable workflows with Geoprocessing History, ModelBuilder and ArcPy;
- recognize risks such as privacy, misleading maps, the ecological fallacy, the MAUP and spatial autocorrelation.

## Who it is for

- students learning GIS or ArcGIS systematically for the first time;
- researchers who need maps and spatial analysis in their work;
- learners in public health, environment, urban planning, business analytics and public administration;
- ArcGIS users who want to move from operating the software to explaining and validating a workflow.

The course takes about **150–210 minutes** and can be completed section by section. It needs only basic file and spreadsheet skills; no R, Python or GIS background is required.

## Software scope

The course follows **ArcGIS Pro 3.x** on the desktop and introduces web maps and content sharing in ArcGIS Online.

- ArcGIS Pro for local data management, cartography, editing, spatial analysis and layouts;
- ArcGIS Online for content management, hosted layers, web maps, pop-ups and sharing;
- ArcGIS Enterprise, Field Maps, Survey123, Dashboards and StoryMaps as parts of the wider platform;
- ModelBuilder, ArcPy and Arcade as an introduction to automation and expressions.

ArcGIS Pro runs on Windows. Learners on macOS or Linux can read all of the material and complete the relevant parts through an organization's remote Windows desktop, a virtual machine or ArcGIS Online. Available tools, extensions, user types, credits and sharing privileges depend on the ArcGIS version and the organization's configuration.

## Course structure

| Module | Core content |
|---|---|
| 1. GIS and the ArcGIS landscape | Types of GIS question; ArcGIS Pro, Online, Enterprise and the app ecosystem |
| 2. ArcGIS Pro projects and interface | `.aprx`, the default geodatabase, toolboxes, Contents, Catalog and Geoprocessing |
| 3. Spatial data models | Points, lines, polygons, rasters, tables, feature classes, layers and common formats |
| 4. Coordinate systems and projections | GCS, PCS, datums, on-the-fly projection, Define Projection and Project |
| 5. Adding and checking data | Folders, geodatabases, Portal, CSV to points, metadata and arrival QA |
| 6. Exploring and symbolizing maps | Symbology, normalization, classification, colour, labels, pop-ups and scale |
| 7. Queries and geoprocessing | Attribute and spatial selection, joins, Buffer, Clip, Dissolve, Intersect and Near |
| 8. Worked practice | A fictional 1 km coverage-gap analysis of community services |
| 9. Editing and integrity | Snapping, domains, subtypes, topology and safe editing |
| 10. Layout and export | Map frame, title, legend, sources, PDF/PNG and map QA |
| 11. ArcGIS Online | Hosted feature layers, views, web maps, permissions and dependency checks |
| 12. Repeatable workflows | History, ModelBuilder, ArcPy, Arcade, logging and naming |
| 13. Troubleshooting | Data sources, coordinate systems, selections, environments, locks, joins, licensing and web permissions |
| 14. Responsibility and spatial inference | Privacy, aggregation, the ecological fallacy, the MAUP, classification and causal limits |
| 15. Exercises and quick reference | Concept questions, a capstone project, glossary, tool cards and a final checklist |

## Running example

The course uses one fully fictional "community service coverage" example:

- communities are polygon features with population and other attributes;
- service facilities are point features;
- a projection suited to the study area, with units in metres, is used;
- a 1 km buffer is created around each facility;
- community centroids and Spatial Join screen for potential coverage gaps;
- input and output counts, coordinate systems, units, edge cases and tool messages are validated;
- results are mapped, and sharing permissions and privacy are discussed.

The R Markdown uses the fixed random seed `20260908` to generate the illustrative communities, facilities, distances and populations, so the teaching figures and result tables are reproducible.

The example covers **straight-line buffers** only. It does not model roads, barriers, entrances, slope, travel mode, opening hours, capacity or cost, so it cannot replace network accessibility analysis or real site-selection decisions.

## Features

- **A complete learning path:** from concepts and operations to validation, delivery and responsible practice;
- **Reproducible illustrations:** fixed teaching data and original figures generated with base R;
- **Readable without ArcGIS:** the HTML opens offline, and ArcPy examples are not executed at build time;
- **Self-contained HTML:** CSS, JavaScript and teaching figures are embedded in the final page;
- **Responsive design:** desktop, mobile and print layouts;
- **Accessibility:** semantic navigation, alternative text, keyboard focus, high-contrast colours and reduced-motion support;
- **Quality-control focus:** every workflow stresses checks on counts, fields, coordinates, units and edge cases;
- **Clear responsibilities:** covers public sharing, sensitive locations, data licensing and the limits of spatial inference.

## File structure

```text
ArcGIS_Study/
├── README.md
├── arcgis_getting_started.Rmd
├── arcgis_getting_started_en.Rmd
├── arcgis_getting_started_en.html
├── styles.css
└── includes/
    └── vlab-brand.html
```

| File | Purpose |
|---|---|
| `README.md` | Project overview, usage, build and maintenance notes |
| `arcgis_getting_started_en.Rmd` | Course source |
| `arcgis_getting_started_en.html` | Self-contained course page |
| `arcgis_getting_started.Rmd` | Source of an earlier, unpublished edition |
| `styles.css` | Colours, layout, callouts, tables, responsive and print styles |
| `includes/vlab-brand.html` | The V Lab · ArcGIS brand component at the top of the page |

## Quick start

### 1. Clone the repository

```bash
git clone https://github.com/LaboratoireV/ArcGIS_Study.git
cd ArcGIS_Study
```

You can also use **Code → Download ZIP** on GitHub and open the extracted folder.

### 2. Open the course

No R or ArcGIS installation is needed. Open `arcgis_getting_started_en.html` in a local browser.

Links to external official resources need an internet connection; all other content, styles and figures are inside the HTML.

### 3. Do the hands-on exercises

To reproduce the steps in ArcGIS Pro:

1. use an organizational account or a licensed ArcGIS Pro environment;
2. choose suitable real data and a coordinate system for your own study area;
3. do not use the placeholder WKID `00000` from the tutorial directly in ArcPy;
4. record parameters, environment settings, tool messages and validation results as the tutorial describes;
5. before publishing web content, check roles, credits, editing permissions, privacy and data licences.

## Rebuilding the HTML from R Markdown

### Requirements

- R;
- `rmarkdown`;
- `knitr`;
- Pandoc (usually bundled with RStudio).

The teaching figures and tables depend only on base R and `knitr`; `sf`, `terra`, ArcPy and ArcGIS are not required.

### Install the R packages

```r
install.packages(c("rmarkdown", "knitr"))
```

### In RStudio

1. Open `arcgis_getting_started_en.Rmd` in RStudio;
2. keep `styles.css` and `includes/vlab-brand.html` at their current relative paths;
3. click **Knit → Knit to HTML**;
4. check the table of contents, figures, tables and folded code in the rendered page.

### From the command line

```bash
Rscript -e 'rmarkdown::render("arcgis_getting_started_en.Rmd")'
```

The current build was verified with R 4.6.1, knitr 1.51, rmarkdown 2.31 and Pandoc 3.8.3. Other recent compatible versions usually work; if a build fails, run `rmarkdown::pandoc_available()` first to check Pandoc.

The output uses:

- `html_document`;
- self-contained resources;
- the Flatly theme with Tango code highlighting;
- a three-level floating table of contents and numbered sections;
- folded code;
- MathML for mathematics;
- responsive, mobile and print styles.

## Maintenance

### Edit the source, not the output

Edit the `.Rmd` source first and then re-render the HTML; do not edit only the generated HTML. When changing the course, check:

- titles, section order and learning goals;
- the data-generation code and random seed of the running example;
- tables, tool parameters, exercises and folded answers;
- figure captions, alternative text and callouts;
- official documentation URLs, ArcGIS version notes and permission descriptions.

### Renaming files

If you rename the HTML file, also update:

- the home link in `includes/vlab-brand.html`;
- the course link and file structure in this README.

### Pre-publication checks

1. The Rmd renders without errors;
2. the HTML has no page-level horizontal scrolling on desktop or narrow viewports;
3. the table of contents and folded answers work;
4. images load fully and have alternative text;
5. the browser console shows no errors;
6. the final HTML does not depend on local absolute paths;
7. no sensitive data, credentials, access tokens or personal information are in the repository.

## Data, code and responsibilities

- This repository is a teaching document project. It contains no `.aprx`, `.gdb` or `.atbx` files, no real GIS data and no ready-to-run ArcGIS Pro project;
- all communities, facilities, distances and populations are illustrative values generated with a fixed seed and do not correspond to real places or people;
- the ArcPy code shows the structure of a workflow only; in an ArcGIS Pro Python environment it needs real paths, coordinate systems, licensing and error handling;
- the course does not replace local spatial-data standards, privacy review, professional network analysis or business decisions;
- straight-line buffers, spatial overlap and visual clustering do not by themselves prove real accessibility or causation;
- when using external data, check its source, date, scale, accuracy, licence, attribution and redistribution terms;
- before making a hosted feature layer or web map public, check all of its dependent layers on the principle of least privilege.

## Licence

The repository does not currently include a `LICENSE` file, so no general open-source reuse licence is granted. To copy, adapt or republish its content, contact the repository maintainer first, and also follow the licence and attribution requirements of Esri, basemaps and any external data.

## Official learning resources

- [ArcGIS Pro Documentation](https://pro.arcgis.com/)
- [ArcGIS Pro Quick-start Tutorials](https://pro.arcgis.com/en/pro-app/latest/get-started/pro-quickstart-tutorials.htm)
- [What is geoprocessing?](https://pro.arcgis.com/en/pro-app/latest/help/analysis/geoprocessing/basics/what-is-geoprocessing-.htm)
- [Introduction to the geodatabase](https://pro.arcgis.com/en/pro-app/latest/help/data/geodatabases/overview/what-is-a-geodatabase-.htm)
- [Coordinate systems, projections, and transformations](https://pro.arcgis.com/en/pro-app/latest/help/mapping/properties/coordinate-systems-and-projections.htm)
- [What is ArcPy?](https://pro.arcgis.com/en/pro-app/latest/arcpy/get-started/what-is-arcpy-.htm)
- [Get started with data in ArcGIS Online](https://doc.arcgis.com/en/arcgis-online/get-started/get-started-with-data.htm)
- [Get started creating maps in ArcGIS Online](https://doc.arcgis.com/en/arcgis-online/reference/get-started-with-maps.htm)
- [Get started with sharing in ArcGIS Online](https://doc.arcgis.com/en/arcgis-online/get-started/get-started-with-sharing.htm)

This is an independent learning module, not official Esri training. Product interfaces and privileges change over time; consult the official documentation for your installed version and organization.

---

Maintained as part of **The V Lab** learning modules.
