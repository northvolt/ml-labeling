# ml-labeling
Instructions and example images for annotation of data.

# Description

Images of material on a roller. During manufacturing, certain type of anomalies and defects can arise. We want to detect and find the locations of these defects. The material should be smooth without any apparent anomalies, but there might be vertical lines which is normally ok.
Note: some images may not contain any defects at all and should be left without any annotation.


# General instructions

You do not have a lot of time to label, so please only focus on the most obvious defects. If you are unsure, skip it or leave the defect unlabeled.


## Region of interest

The images show material on a roller. The outmost parts (left and right) are the roller. We are only interested in the material and the bare foil. Where the region of interest is will vary slightly in each image:
![Region of interest](./vision-anomaly-detection/examples/roi-unpressed.jpg)

Any defect or anomalies outside of this region are irrelevant and should not be labeled.

### Good examples

There are 3 categories of defects: anomaly, knurling and foil-anomaly:

1. anomaly: any fairly obvious dent, hole or scratch in the region of interest, but not on the bare foil:
![anomaly](./vision-anomaly-detection/examples/anomaly/2020-07-02T08-42-00.650174555Z.jpg)
![anomaly](./vision-anomaly-detection/examples/anomaly/2020-07-05T07-13-44.506911644Z.jpg)


2. knurling: a special type of anomaly where a series of bumps or wrinkles appear close to the edge of the material:
![knurling](./vision-anomaly-detection/examples/knurling/2020-07-06T12-37-15.649572202Z.jpg)


3. anomaly-edge: anomalies that occur in the bare foil of the photos
![anomaly-edge](./vision-anomaly-detection/examples/anomaly-bare-foil/2020-07-02T07-37-28.67626241Z.jpg)


### Bad examples

We do not care about defects that are not in the region of interest, for example:

![bad bbox](./vision-anomaly-detection/examples/bad-bbox/2020-07-01T10-57-45.046169911Z.jpg)
