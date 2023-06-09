---
title: Software navigation
nav_order: 3
---

# Software navigation
{: .no_toc }

This section presents information related to PathFinder's interface, explaining the layout and how the case data is organized in the software.

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

### Opening a case
A PathFinder case is opened informing its folder to the interface. After opening the software, a window will be displayed for the insertion of the case directory.

<img src="./assets/inform_case.png" alt="" />

After inserting the case directory, click open to load the case data. If the folder informed does not contain any data related to the software, the interface will ask if an empty case should be created from scratch.

### A quick PathFinder layout overview

The PathFinder tabs have standard layouts, allowing quick learning on the study configuration workflow.

<img src="./assets/layout_overview_v2.png" alt="" />

The interface can be divided into sections, each one containing a group of controls and/or data for configuration.

1. Basic data registry where it can be visualized and configured
2. Menu containing data options such as filters, datasheet interface, layout configuration and data adding and removing controls
3. Window that lists subsections that can be enabled or disabled for visualization
4. Attribute configuration section for attributes that require association with other collections
5. Treeview of the interface tabs

#### Adding and removing elements

Elements can be added or deleted from the case in ```2``` in the ```registry``` area.

#### Exporting and importing data to Excel

PathFinder allows importing and exporting data to datasheets. It can be done in ```2``` in ```Get & transform data``` area.

#### Associating elements

Some attributes are used to link collections, e.g. the ```candidate``` collection which requires association to ```spatial constraint``` and ```map``` data. These can be configured in ```4```.

#### Running PathFinder

The model can be executed in the ```Run``` tab presented in ```2```. 

### PathFinder tabs

#### Geographical data

Geographical data holds data whose definition rely on geographical coordinates. The collection and associated subtabs defined in ```Geographical data``` are:

| Subtab | Collection | Description| Relates to |
|--------|------------|------------|------------|
| Bus    | Bus collection | Defines electical buses for candidate origin-destination routes | Candidate collection |

#### Candidate data

Candidate data holds data related to transmission line candidate definition, which includes origin-destination geographical coordinates of each candidate, spatial constrains and data maps. The collection and associated subtabs defined in ```Candidate data``` are:

| Subtab | Collection | Description| Relates to |
|--------|------------|------------|------------|
| Candidate | Candidate collection | Defines transmission line candidates for the study | - |
| Spatial constraint | Spatial constraint collection | Defines candidate constraints for the study | Candidate collection | Candidate collection |
| Map | Map collection | Defines map elements for a candidate | Candidate collection |

#### Electrical data

Electrical data holds data related to transmission line elements, such as cable and transmission towers characteristics. The collections defined in ```Electrical data are```

| Subtab | Collection | Description| Relates to |
|--------|------------|------------|------------|
| Cable | Cable collection | Defines power cable characteristics| Tower arrangement collection |
| Tower | Tower collection | Defines transmission tower characteristics| Tower arrangement collection | Candidate collection |
| Tower arrangement | Tower arrangement collection | Defines transmission lines characteristics | - |