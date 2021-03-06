---
title: exporting and uploading images with metadata
id: export-metadata-upload
draft: false
weight: 50
author: "people"
---

Changes to an image are not saved directly to the image file as they are in a regular (raster) image editor. Rather, darktable is a non-destructive editor, which means that all changes are recorded in darktable's library database, and the original image is left untouched. Therefore, you need to export images in order to bake your processing options and metadata changes into an output file that can be distributed outside of darktable.

Images are exported using the [export](../../module-reference/utility-modules/shared/export.md) module which is available in the lighttable and darkroom views. This module offers a lot of options, but by far the most common use is to "save my developed raw image as a JPEG".

When exporting images in darktable, there are two basic questions you need to answer:

- _Where shall I send the exported images?_ Most often you will choose to write the files to a folder on your local disk, but other options include writing them to a LaTeX photo book template or sending them to another program such as [Hugin](http://hugin.sourceforge.net/) (for panorama stitching) or [GIMP](https://www.gimp.org/) (for further editing).

- _In what format shall I save the exported images?_ This covers not only the image file format (JPEG, PNG, TIFF, OpenEXR etc.) but also the quality, compression, resolution, picture profile settings and which metadata to embed in the exported image.

The most common steps would therefore be:

1.  Select one or more images in the lighttable view

2.  Choose the target storage and file format

3.  Set the maximum image width and height. Leave the width and height maximums at zero to export at full resolution.

By default, each image will be saved to local disk as a high-quality JPEG at full resolution. For further information on all the available export options, please refer to the [export](../../module-reference/utility-modules/shared/export.md) module reference section.
