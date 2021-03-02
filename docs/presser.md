# Presser
Instructions and example images for annotation of presser image data.

# Description

Images of material on a roller. During manufacturing, certain type of anomalies and defects can arise. We want to detect and find the locations of these defects. The material should be smooth without any apparent anomalies, but there might be vertical lines which is normally ok.
Note: some images may not contain any defects at all and should be left without any annotation.


# General instructions

You do not have a lot of time to label, so please only focus on the most obvious defects. If you are unsure, skip it or leave the defect unlabeled.


## Region of interest

The images show material on a roller. The outmost parts (left and right) are the roller. We are only interested in the material and the bare foil. Where the region of interest is will vary slightly in each image:
![Region of interest](../images/presser/roi-unpressed.jpg)

Any defect or anomalies outside of this region are irrelevant and should not be labeled.

# Types of defects

There are 3 categories of defects: anomaly, knurling and foil-anomaly.

1. anomaly: any fairly obvious dent, hole or scratch in the region of interest, but not on the bare foil:
![anomaly](../images/presser/anomaly/2020-07-02T08-42-00.650174555Z.jpg)
![anomaly](../images/presser/anomaly/2020-07-05T07-13-44.506911644Z.jpg)


2. knurling: a special type of anomaly where a series of bumps or wrinkles appear close to the edge of the material:
![knurling](../images/presser/knurling/2020-07-06T12-37-15.649572202Z.jpg)


3. foil-anomaly: anomalies that occur in the bare foil of the photos
![foil-anomaly](../images/presser/anomaly-bare-foil/2020-07-02T07-37-28.67626241Z.jpg)

Moreover, the images could show different material with certain characteristics. For example, the wrinkles in the bare foil as shown in the image below should not be treated as a foil-anomaly. The focus with respect to foil-anomalies should be on more local anomalies as visualized in the foil-anomaly example above. 

![unpressed-wrinkles](../images/presser/unpressed.png)


### Good examples
Don't spend too much time annotating everything perfect, however try to label as few non-defect pixels as possible:

#### Anomaly 

<img src='../images/presser/anomaly-unannotated.png' width="200" height="200" /> <img src='../images/presser/anomaly-annotated.png' width="200" height="200" />

#### Knurling 
<img src='../images/presser/knurling-unannotated.png' width="200" height="200" /> <img src='../images/presser/knurling-annotated.png' width="200" height="200" />

#### Foil anomaly
<img src='../images/presser/foil-anomaly-unannotated.png' width="200" height="200" /> <img src='../images/presser/foil-anomaly-annotated.png' width="200" height="200" />


### Bad examples

Area around annotated defect is too large:

<img src='../images/presser/bad-bbox/anomaly-bad-annotation.png' width="200" height="200" />

We do not care about defects that are not in the region of interest, for example:

![bad bbox](../images/presser/bad-bbox/2020-07-01T10-57-45.046169911Z.jpg)

### Labeling example 
Image pre labeling: 

![pre-labeling](../images/presser/unannotated.png)

Image after labeling, where green refers to an anomaly, blue refers to knurling and orange refers to foil-anomalies:

![post-labeling](../images/presser/annotated.png)

