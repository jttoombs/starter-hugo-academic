---
title: Microscale computed axial lithography
summary: A light-based 3D printing process based on computed axial lithography.
# tags:
#   - Deep Learning
date: '2022-1-3'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: 'Image credit: Joseph Toombs'
  focal_point: ''
  placement: 1
  preview_only: false


authors:
  - admin

# links:
#   - icon: twitter
#     icon_pack: fab
#     name: Follow
#     url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ''
---



## Micro computed axial lithography (MicroCAL)

![](images/microcalbanner.jpg)

MicroCAL is a light-based 3D printing based on the tomographic exposure principles of CAL. 

### Optical layout

The MicroCAL has a custom laser-based optical system. A diode laser is launched into an optical fiber to homogenize the output irradiance profile. The fiber is collimated and expanded. The beam is directed onto the digital micromirror device (DMD). The digital mask is imaged into a rotating vial of photosensitive material. The digital projection images are refreshed in sync with the rotation of the material. The point spread function (PSF) width was measured by projecting a mask of an edge, capturing images of the edge with a CMOS sensor, and using a supersampling algorithm. The PSF was about 4 µm full-width half-maximum. 

![](images/microcallayout.jpg)



### Roughness

In this study, a nanocomposite resin was used. The nanocomposite composes spherical silica nanoparticles and a monomer binder. The binder is burnt out in a thermal treatment process after printing is completed. The roughness of rectangular beams printed by microCAL and other layer-based printing methods was measured and compared. In metrics: arithmetic mean surface roughness, valley height, and surface gradients, MicroCAL showed the smallest magnitude. 

![](images/microcalroughness.png)


### Printing

Coordination of the rotation stage and DMD is done with a custom Python software running on a PC. The laser is controlled by a microcontroller which is controlled by the PC via serial communication. Prints require approximately 45-90 seconds of exposure time. Polymeric and silica glass parts were printed with minimum feature sizes of 20 and 50 µm.

![](images/microcalpolymer.jpg)

![](images/microcalmicrolens.jpg)

![](images/microcalmicrofluidic.jpg)
