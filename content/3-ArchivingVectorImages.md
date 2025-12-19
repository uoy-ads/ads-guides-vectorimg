---
authors:
  - name: null
---

# 3 Archiving Vector Images

## 3.1 Deciding what to archive

As mentioned in Section 1, vector images are often created in archaeology as a step within a larger project workflow either as the output from a data processing application or as a stage towards producing high quality illustrations. In both cases such files represent the creation of a 'final product' image, usually for inclusion within a project report, and many are often formatted in terms of a printed page. A further step may even see vector images rasterised as JPG or TIFF files prior to their inclusion within a document. It is therefore important for the data creator to evaluate the importance of the vector image within the workflow and to decide whether the file in question has reuse value in that particular format. In cases where the image exists in both its source (e.g. CAD) and derived (e.g. raster images) forms then it may be decided that the vector image is not retained and archived.

In addition to the image itself, many vector image applications allow the inclusion of scripts (e.g. JavaScript, AppleScript or VBScript in Illustrator) within files. Scripting within such files aims to automate or simplify tasks at the creation or editing stage and are not considered to be a core component of the vector image. If such scripts are seen as being worth preserving then they should be stored and documented separately to the image.

## 3.2 Deciding how to archive

__Significant Properties__

As with other file types, when archiving vector images it is essential that the core significant properties of the file are identified and maintained within the chosen format. The JISC report 'The Significant Properties of Vector Images' [@coyne2007significant] more than adequately details the properties that should be identified and maintained when archiving vector images and these will only be briefly outlined here.

As would be expected, the significant properties of a vector image revolve around the geometry of the image, the vector objects and their relationships, and the conventions (colours, line types and weights) used within the file and maintaining the appearance of these throughout file migrations and archiving. The following elements are those that should be monitored during the archiving of vector files:

* Points, paths (open or closed) and objects (e.g. text, referenced or embedded objects) 
* Basic shapes / Primitives (e.g. rectangle, circle, ellipse, etc.)
* Image structure (i.e. the grouping and layering of objects)
* Clipping and masking
* Transformations and Coordinate Systems (if present, though these are mostly present in GIS and CAD vector files)

In addition to ensuring that these specific vector elements remain physically present within a file in the same format, there are a number of obvious properties that can be applied to these. Where standardised conventions exist and have been followed (such as specific meanings associated with certain line colours or dash types) it is essential that these properties and formatting is maintained in archived files. Such properties include:

* Line width, cap and join types
* Miter limit
* Dash pattern and offset
* Colour
* Opacity
* Rendering
* Interior definition
* Gradient and gradient smoothness
* Pattern
* Text attributes such as font size, weight or style.

Interestingly, the JISC report has proposed a potential hierarchy of significant properties which may be used to assess which properties to prioritise if a file does not easily transfer to a preservation format [@coyne2007significant, 41].

Unfortunately there is no simple, objective way to compare between original files and migrated versions other than visually assessing that all elements are rendered in the correct way. When migrating a file to a new format, aside from the obvious visible elements, it is also important to check for hidden information such as invisible objects or layers and to assess the relevance or suitability of these for archiving. Linked data, such as embedded raster files or external fonts, may also be present in the original image and the appearance of such data should be maintained through any file migration. Successfully preserving a vector file is largely dependent on the nature of original, its complexity and whether it contains pure vector data or incorporates raster data as well. Such mixed files may require the separation of data types into suitable preservation formats.

__File Formats__

```{list-table}
:header-rows: 1

* - Preservation Format
  - Requirements
* - .svg
  - As an open xml-based standard, SVG is the preferred format for the long-term storage and preservation of vector images.
* - .pdf/a
  - Although suitable for preserving vector graphics, pdf/a is recommended as a 'last resort' format as, although the format retains the vector nature of the file, it does reduces the reuse potential to simple 'view only'.
```

## 3.3 Metadata and Documentation

Metadata for vector images is discussed in detail in 'The Significant Properties of Vector Images' [@coyne2007significant], from which the elements below are taken, and on the JISC Digital Media page discussing 'Metadata and Digital Images'. The elements below are largely [Dublin Core](https://www.dublincore.org/) elements which are most usefully generated by the image creator. In addition, some technical elements are suggested (only a subset of those presented in 'The Significant Properties of Vector Images') which may be optionally completed by the data creator.

```{list-table}
:header-rows: 1

* - Element
  - Description
* - Identifier
  - A unique identifier for the image, usually the filename
* - Title / Caption
  - The title of the image or a suitable caption
* - Description/Purpose
  - Description of the image
* - Creator
  - Name of image creator
* - Date
  - Creation date
* - Rights
  - Details of copyright or other rights and holder details
* - Keywords
  - Keywords e.g. period, site or feature terms. Use suitable thesauri where they exist
* - Provenance/Relationship to other documents
  - Description of where the image originated and how (if relevant) it is related to other files
* - Conventions
  - If applicable and not contained within the document, an explanation of all conventions used (colours, layers, line styles, line weights, etc.)
```

__Additional Basic Technical Metadata__

```{list-table}
:header-rows: 1


* - Element
  - Description
* - File Format and Version
  - e.g. SVG 1.1
* - File Size
  - Size of the file in bytes
* - Software
  - Software used to create the image e.g. Adobe Illustrator
```

## 3.4 Structuring your archive

Vector images should be structured logically and in a matter which suits the particular project. A file structure may reflect a specific site or feature or separate instances of fieldwork or photographic survey. Where metadata is to be preserved, it is suggested that it be extracted and stored in a simple text (plain or delimited) or XML structure in a "documentation" folder alongside the preserved images.