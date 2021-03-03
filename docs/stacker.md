# Stacker
Instructions and example images for annotation of stacker image data.

# Description

The task is to annotate defects on the electrodes during stacking in cell assembly. The defects are annotated by the use of an external tool available as a service on Amazon Web Services. If you're interested in helping out, let Martin Hwasser know and he will send an invite.

The maximum time to spend annotating one image is set to a few minutes, if a task is completed before time exceeds simply press _Submit_ in the bottom left corner and proceed.

__N.B.__ if there are no defects present in an image, select _Nothing to label_ in the bottom left corner followed by _Submit_ in order to move on to the next image. In case of uncertainty, press _Decline task_ to move on to the next image.

## Region of interest

The region of interest regarding this task is the coated area as presented in the Figure below. Hence, in the case of a tab being present, this should not be annotated.

![Region of interest](../images/stacker/roi.jpg)

Any defect or anomalies outside of this region are irrelevant and should not be labeled.

## Camera artefacts

Due to the nature of the stacker machine i.e., that it runs in a non-continous manner with lots of stops, some images suffer from camera specific artefacts which should not be annotated as defects. Below are two examples of aforementioned artefact:

![Artefact1](../images/stacker/artefact1.jpg)

![Artefact2](../images/stacker/artefact2.jpg)


### Annotation examples

Don't spend too much time annotating everything perfect, however try to label as few non-defect pixels as possible.

#### Example 1

Given an image to annotate:
![Example image](../images/stacker/unlabeled1.png)

The defect is located:
![Example image defect arrow](../images/stacker/unlabeled1-arrow.png)

The defect is annotated:
![Example image defect arrow](../images/stacker/labeled1.png)

#### Example 2

Given an image to annotate:
![Example image](../images/stacker/unlabeled2.png)

The defect is located:
![Example image defect arrow](../images/stacker/unlabeled2-arrow.png)

The defect is annotated:
![Example image defect arrow](../images/stacker/labeled2.png)
