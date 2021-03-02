# Stacker image annotation/labeling

## Description

The task is to annotate or "label" defects on the electrodes during stacking in cell assembly. The defects are annotated using an external tool in Amazon Web Services. Once you are done labeling an image, simply press _submit_.

**Important:** if there are no defects present in an image, select _Nothing to label_ and then _submit_ to move on to the next image. If you are uncertain, you can choose _Decline task_ to move on to another image.

### Region of interest

We are only interested in defects on the coated area (see image below). If a tab should be folded on top of the material, annotate it as a defect or decline the task.

![Region of interest](../images/stacker/roi.jpg)

Any defect or anomalies outside of this region are irrelevant and should not be labeled.

### Camera artefacts

Many images contain long horizontal lines. These are camera specific artefacts due to machine starting and stopping and should not be annotated as defects. Below are two examples of this phenomenon:

![Artefact1](../images/stacker/artefact1.jpg)

![Artefact2](../images/stacker/artefact2.jpg)

### Annotation example
Given an image to annotate:
![Example image](../images/stacker/full-size.png)

The defect is located:
![Example image defect arrow](../images/stacker/full-size-arr.png)

The image is zoomed and the defect is then annotated:

<img src='../images/stacker/unlabeled-defect.png' width="200" height="200" /> <img src='../images/stacker/labeled-defect.png' width="200" height="200" />

### General advice
Don't spend too much time annotating a defect perfectly, but try to make sure that the entire defect is inside the colored area and that the colored area does not extend much beyond the defect. Once you are used to the tool, labeling should not take more than a minute or two.
