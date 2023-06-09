# Floor Plan Generator

The core idea of this project is to dynamically create floorplans using Generative Adversarial Networks (GAN). The networks generate floorplans examples based on input by a user. The user would be able to make adjustments and then move through various stages of floorplan design.

The dataset process is split into several steps:

 - __dataset_builder.GeoDataGenerator__ creates geodataframe from the txt files dataset.
 - __dataset_builder.groundplan__ module creates ground plan images.
 - __dataset_builder.ImageFloorplanGenerator__ creates floor plan images.
 - dataset_builder.ImageStructureGenerator module creates structure images.
   
__ImageFloorplanGenerator__ and __ImageStructureGenerator__ can also be done as a single step, this is done with the following generator:

- __dataset_builder.ImageSingleStepGenerator__
