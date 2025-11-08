# Manual for garments published according to OSPP standard

> [!TIP]
> See GitHub's markdown table of contents above for quick navigation.


## Introduction

This manual contains guidelines and technical specifications required for patterns and visualisations to be published according to Open Source Production Patterns (OSPP) specifications, as originally described by Rickard Lindqvist.

The patterns of the styles shared through this platform should be ready for production. I.e. include all information such as seam allowance, notches, grading etc needed for industrial production.


## Organising pattern pieces in 2D window

- The 2D patterns should be grouped and organised so that pieces can be easily recognised in the 2D window, please see the layout below.

- Use the "Symmetric Pattern" function on all pattern pieces that are symmetrical.

- Check that the grain lines are marked correctly.

<img src="images/2.png" alt="Example: Top pieces">|<img src="images/1.png" alt="Example: Bottom pieces">
-|-
Example: Top pieces | Example: Bottom pieces


## Annotations and names on pattern pieces

Use the pattern annotation function to add information to the pattern pieces if needed, i.g. ease, pleats etc.

Give each pattern piece explanatory names in the property editor (not as annotations) so that they can be recognized in the 2D window and after the have been printed out for production, eg. RHS Front, Back, RHS Sleeve, Top Collar etc. Denote Right and Left with RHS (right hand side) or LHS (Left Hand Side).

<img src="images/3.png" alt="Example of annotation">|<img src="images/4.png" alt="Naming pattern piece">
-|-
Example of annotation | Naming pattern piece


## Fusing

Fused parts need to be marked for production. Use the bond function for this.

Bond the full piece if it should be block fused, i.e fused before cutting (this normally applies to pocket pieces, waistbands, jacket collars etc.).

|<img src="images/6.png" alt="Example: Block fused pattern piece">|
|-|
Example: Block fused pattern piece


### Fusing inside of a pattern piece

- Create an internal shape inside of a pattern piece.
- Choose the Bond function under "Property Editor". Then the pattern for the fusing is automatically created in the Print Layout Bond window.

<img src="images/5.png">|<img src="images/8.png">|<img src="images/7.png">
-|-|-


### Fusing outside of/along a pattern outline

- Fusing pieces must be 2 mm smaller than the seam allowance in order work well in the fusing machine.

- Right click on the selected lines and use "Offset as internal line (Reversed Direction)" to create the outlines of the fusing piece.

- Complete the fused area by drawing internal lines. If needed, right click on the overlapping points and join them to create an internal shape, mark it and choose Bond in the property editor.

- Check the grain line of the fusing under the fusing tab in the Print Layout mode (scroll down menu in the top right corner).

|<img src="images/new_image_001.png">|
|-|


## Seam allowance

All pattern pieces should include a seam allowance for the physical production.

Add the proper seam allowance according to the sewing method with the seam allowance tool in the 2D window.

| | Stitch type | Seam allowance | Description |
| :-: | - | - | - |
|<img src="images/15.png" width="75%">| 1-Needle Lockstitch | 1 cm | 1 cm is generally used for 1-needle lockstitch seams. |
|<img src="images/16.png" width="75%">| Stiched and turned 1-Needle Lockstitch | 0,5 cm | 0,5 cm is generally used for stitched and turned 1-needle lockstitch seams, eg. edges of collars and cuffs. |
|<img src="images/17.png" width="75%">| 4-thread overlock | 0,7 cm | The overlock seam is generally 0,5 cm wide. 2 mm margin is added to be cut away when sewing. |
|<img src="images/18.png" width="75%">| 5-thread safety stitch | 1,2 cm | The overlock plus chainstitch seam is generally 1 cm wide together. 2 mm margin is added to be cut away when sewing. |
> Example of seam allowance according to different stitching.

> [!NOTE]
> The seam allowance is only for joining seams and part of pieces "inside" of a seam, generally NOT for fold and hems. See explanation below.


### Seam allowance for hems and folds

To facilitate simlulation, and to be able to adjust stylelines in Jinny (or in the 3D window), we recommend hemfolds are marked as seam allowance.

Make sure that the correct seam allowance angles are used if the ends are not 90 degrees.

|<img src="images/19.png">|
|-|

However, when handling hemfolds like this the inside of the hem is not visible in the 3D visualisation or rendering.

**If** there is a need for inside hem visualisation, e.g. if the front and back side of the fabric has different textures or colours, add the by unfolding the hem. Use the fold tool to make a nive hemfold and add seamallowence as on the image below.

|<img src="images/20.png">|
|-|


### Seam allowance for darts

If darts should not be cut open, i.e up to 2 cm wide, use internal lines at each dart leg and in the middle. Apply fold values to the internal lines and fold in desired direction. Use the mesh tool from the 3d menu to subdivide the mesh of the dart to make it smooth. (below left)

If the dart should be cut open, leave the dart open and add seam allowance (below right).

|<img src="images/new_image_002.png">|<img src="images/new_image_002b.png">|
-|-
Example *not* cut-open dart | Example cut-open dart


## Topstitches

Use, as far as posible, the pre-defined topstitches with ISO-codes suplied by CLO. Topstiches for OSPP should be colored white.

Place, as far as possible, toptitches on the outlines of the patterns and offset if needed. **Avoid unnecessary internal lines.**

|<img src="images/26.png">|
|-|


## Trims

### Buttons

- Add button and bottonholes using the tool in the 3d window. Make sure to lock the button into position if possible.

- Adjust size according and color the buttons white.

- Mark drillhole on correct facing of the fabricpiece.


### Buckles and other imported 3d objects

- Add trim infomation about the object in the property editor and tick off *include in techpack*.

- Adjust size according and color the buttons white or black.


### Elastics, cords and velcro pieces

- Add piece as a regular patternpiece, name and archive it.

- **Change from pattern to trim** in the property editor, tick off *include in techpack* and choose trim classification.

- Add fabric and texture matching the trim.

|<img src="images/new_image_003.png">|
|-|


## Notches and drill holes

### Notches

- ONLY add notches that are necessary for the physical production to your pattern. Notches should be helpful when sewing, i.e **no** notches for marking centre front, waist lines, places of measure etc.

- Place notches on long and/or curved lines notches every 20-40cm to facilitate assembling.

- Hem and fold lines should be marked with notches.

<table><tr><td><img src="images/new_image_004.png"></td></tr><tr><td>

1. Joining notches.
  > [!NOTE]
  > Always place a notch 8 cm from sideseam front pcs and front side of sleeve.
2. Notches to mark foldline.
3. Notches to mark folded hemline.
</td></tr></table>


### Drill holes

- Pocket placements, end of darts etc. should be marked with drill holes.

- Create drill hole as a 3mm **baseline circle** with a cross inside. (Baselines has to be used as internallines are *not* printed in production.)

- Drillholes that mark the placement of details should be placed 3 mm inside of outline.

- Place drill holes 1 cm away from the dart point inside the dart.

<img src="images/new_image_005.png">|<img src="images/new_image_006.png">
-|-
Example: Drillholes in pocket corner | Example: Drillholes in dart point

## Point of measure (POM)

- Measurements are needed to control the garment production and of the grading. Only mark measurements that are needed to maintain quality and that can be taken on a finished garment but at least the measurements shown in the example below.

- Choose suitable measurements based on the design and of the garment.

- Note: Please check the [CLO manual](https://support.clo3d.com/hc/en-us/articles/360025716774-Create-POM) for further instructions.

|<img src="images/37.png">|
|-|


## Grading

Before grading make sure that the pattern is cleaned up and only contains nessesary lines and points for production and 3d visualisation. Sectionpoint should only appear in corners, where lines intersects amd with notches.

- Garments must be graded in suitable steps and size range for the production.

- Download already graded styles from the OSPP archive for references if needed.

- Generic principal guidlines for tops and bottoms are provided below

  Blue lines shows growth only vertical or horisontal.
  
  Red lines shows growth vertical and horisontal based on position in the grid.

<img src="images/new_image_007.png">|<img src="images/new_image_008.png">|<img src="images/new_image_009.png">
-|-|-

### Example: Grading suggestion for shirt

> [!NOTE]
>
> Differences between each alphabetic size (chest circumference 6cm)

|<img src="images/new_image_010.png">|
|-|


### Example: Grading suggestion for pants (jeans)

> [!NOTE]
>
> Differences between each inch size, i.e 29, 30. 31, 32 etc

|<img src="images/new_image_011.png">|
|-|

Please check the [CLO manual](https://support.clo3d.com/hc/en-us/articles/360000742948-Apply-Grading) for further instructions if needed.

- Use POM-list to control the grading.

|<img src="images/new_image_012.png">|
|-|

> [!IMPORTANT]
> 
> *After grading* check the seamlengths in each size after grading has been applied. Adjust to make all seams correspond if needed.


## Visualisation

- Use the fabric texture from the [`Default_OSPP_Fabric`](resources/Default_OSPP_Fabric.zfab) file found in the resources folder.

- The woven checked lines should indicate scale and grain direction. The black lines indicate the grain direction and the blue lines indicate the cross-grain direction. Each square should measure 10x10cm.

- Use fabric properties that are suitable for the design (can be changed in the bottom of the property editor).

<img src="images/54.png">|<img src="images/55.png">|<img src="images/56.png">
-|-|-


## Preparations for uploading and rendering

- After setting up the visualsation and pattern save it in 2 version:
  1. version called "name_workfile.zprj" for rendering images from.
  1. version only with garment called "name_upload.zpac" for uploading.
 
-  The workfile is for rendering the thumbnail and subimages from.

-  The workfile should include both the assembled garment and the flat pattern on the floor. To get the flatpatternlayout, copy the pattern, select it, right click and choose "reset 2D arrangments", delete selected sewings.

-  Place the flat pattern under the avatar flat on the ground (avoid "footprints" on the fabric from the avatar).

-  Turn of avatar visibility.

-  Set particle distance to 5, and simulate with high-res before rendering.

-  Open and use the rendering properties presets attached to the manual.

|<img src="images/57.png">|
|-|


## Rendering of thumbnails and subimages

Thumbnail, both garment and pattern visible | Subimages
-- | --
Apply presets from manual. | Apply presets from manual.
Format 600x800px. | Format 600x800px.
The thumbnail should show both the assembled garment and the flat pattern on the floor. | Subimage 1 should show the assembled garment only
| | Subimage 2 should show the flat pattern on the floor.
Camera angle and positioning as below. | Camera angle and positioning for flat pattern as below.

<img src="images/58.png">|<img src="images/60.png">|<img src="images/59.png">
-|-|-


## Sharing OSPP designs

An OSPP garment design should include:

- Upload file (Zpac file according to specifications **without** avatar)

- Workfile (Zprj file with avatar and a copy of pattern flat on the floor)

- Rendered images containing Thumbnail and 2 subimages.

All files should be added to a git repository and published on GitHub. (Keep individual files under 100 MB.)

