---
authors:
  - name: null
---

# 2 Creating Vector Images

## 2.1 General Considerations

As outlined in the previous section, unlike common raster images such as photographs, many vector images are derived from data created or held in other applications such as CAD or GIS (which in turn is often derived from a range of data collection techniques such as geophysical survey or laser scanning). It is advised that if an image is derived from another dataset, e.g. a CAD file, then preservation of the original file should take precedence over the derived image. In many cases, derived vector images are frequently used for illustration purposes in documents such as project reports and so are also present elsewhere in a project dataset.

Where images have been created natively within a vector graphics package, or where a derived file (e.g. an illustration with added features e.g. descriptive text) is seen as being worth preserving in its own right, then the guidance in this chapter should be followed. The table below outlines a number of common formats used for the creation of vector images together with their suitability for use in the long-term preservation of the file.

## 2.2 File Formats

```{list-table}
:header-rows: 1

* - Format
  - Properties/Technologies
  - Description
  - Recommendations
* - Adobe Illustrator (.ai)
  - A proprietary, primarily 2D, layer-based raster/vector format.
  - The format itself has changed throughout its history with early versions being based on PostScript. 3D capabilities were introduced with Illustrator CS. Although popular and a market leader, the file format is not well supported by other applications.
  - Not suitable for preservation.
* - CorelDraw (.cdr)
  - A proprietary layer-based 2D format
  - Similar to the Illustrator .ai file format, .cdr can hold both raster and vector data.
  - Not suitable for preservation.
* - PostScript (.ps)
  - A programming language, developed by Adobe, to describe the appearance of text and images in a device-independent manner.
  - The format has a number of derivatives, notably EPS and PDF (see below), the latter of which has slowly supplanted Postscript in terms of popularity.
  - Although potentially suitable for preservation, Postscript is no longer commonly used and newer alternatives such as PDF/A present a more robust preservation format.
* - Encapsulated PostScript (.eps, .epsf and .epsi)
  - Essentially EPS is a restricted, self-contained PostScript file that can embedded into another document.
  - EPS may contain vector or bitmap data and fonts and a preview image is normally included. EPS headers often contain a version number and some programmes may reject a file if the version number is absent.
  - As with Postscript, EPS is considered as not suitable for preservation due to the availability of more appropriate formats.
* - Portable Document Format (.pdf, .pdf/a, .pdf/e, pdf/x)
  - PDF is a subset of Postscript developed by Adobe
  - Limited to purely page description, .pdf incorporates a number of specialised subsets designed for specific purposes (e.g. archiving or engineering). The PDF format is designed primarily for platform-independent document sharing. PDF content can be ASCII text in some cases but the files are more commonly compressed and are therefore binary.
  - PDF/A profile files are considered suitable for preservation but, due to the restrictions required to make them largely self-contained, may not be suitable for all types of content.
* - Scalable Vector Graphics (.svg)
  - An open standard, XML-based format used to describe 2D vector graphics and developed by the [W3C](https://www.w3.org/groups/wg/svg/).
  - In many cases SVG is used on the web together with Javascript to provide certain functionality. In such cases the container (i.e. the web page) and svg must be treated as linked files and both preserved and/or presented together.
  - Suitable for preservation.
* - Computer Graphics Metafile (.cgm)
  - A 2D raster/vector format of some vintage and a documented standard format ([ISO/IEC 8632](https://www.iso.org/standard/32378.html)).
  - A subset of the format, [WebCGM](https://www.w3.org/TR/2010/REC-webcgm21-20100301/), has been developed over recent years by the W3C as a version of the format suitable for use of the web.
  - As an open documented standard, WebCGM has potential as a preservation format but is largely superseded by SVG.
* - Microsoft Windows Metafile (.wmf, .emf)
  - A proprietary vector-based file format that uses Graphics Device Interface (GDI) commands to render an image.
  - EMF is an enhanced version of the WMF standard for 32-bit architectures.
  - Not suitable for preservation.
* - WordPerfect Graphics Metafile (.wpg)
  - A 2D graphics meta format capable of storing bitmapped, vector graphics or EPS data.
  - WordPerfect 5.0 and earlier can store either bitmap or vector image data, but not both at once.
  - Not suitable for preservation.
* - Macintosh PICT (.pict, .pic, .pct)
  - A meta-format developed by Apple in 1984 that can store both bitmap and vector images.
  - The file contains all the QuickDraw commands used to draw the image. PICT files containing only one bitmap are supported under Windows using QuickTime for Windows.
  - Not suitable for preservation.
* - Macromedia Flash (.swf, .fla, .swd, .flv, .swc, .swt, .flp)
  - A 2D vector-based animation format optimised for web delivery.
  - The format specifications are freely available but certain elements are still believed to be closed. Flash files are not limited purely to vector images but incorporate scripting and other multimedia to provide a range of functionality.
  - Not suitable for preservation. 
* - Macromedia Freehand (.af)
  - A popular illustration package that uses a bitmap vector hybrid file type.
  - The file format has changed substantially, resulting in some problems when migrating early versions. As of 2007, development and support for Freehand was discontinued although files are supported within Adobe Illustrator.
  - Not suitable for preservation.
* - Micrografx Designer
  - .drw, .dsf
  - A vector/bitmap-based programme aimed more at technical than artistic drawing.
  - Not suitable for preservation.
```

__Other Formats__

In addition to the files discussed above, there are a number of other vector formats that data creators should be aware of.

The most obvious groups excluded from the above table are vector formats associated with CAD and GIS applications. Formats such as DXF, DWG and SHP are frequent components of archaeological projects and are dealt with elsewhere in these Guides in the appropriate [CAD](https://doi.org/10.5284/k5hd-hj61) and [GIS](https://doi.org/10.5284/vk98-3372) chapters.

The growing popularity of the Open Office suite, including the Draw application, presents the possibility that data creators may start to create and store images in Draw's ODG format. The format, while XML-based and part of the OASIS Open Document specification, is not well supported by other applications. Draw does, however, support export to SVG as well as a number of other formats and, at present, these are recommended for long-term storage of files.
