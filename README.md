# Phase unwrapping pipeline

This phase unwrapping pipeline is useful to unwrap the phase part of a suscptibility-weighted imaging (see figure below). The unwrapped phased image can be used in multiple sclerosis to detect paramagnetic rim lesions (PRLs) that corresponds to chronic active lesions. 

![Phase Unwrapping Pipeline](/home/stluc/Pictures/BMAT_Pictures_vf/phaseUnwrappingPipeline.png)

## Utilization

![Phase Unwrapping windows](/home/stluc/Pictures/BMAT_Pictures_vf/ph_un_win.png)

You will find above an image of the window of this pipeline. This window allows the user to enter for which subjects and sessions he wants to unwrap the phase image, and then to launch the pipeline. By default, this pipeline will apply the image processing on the image with the following sequence name: *acq-WRAPPED_part-pahse_T2starw*. If you want to change the name of the sequence on which to run this pipeline, you can change that in the *phase_unwrapping.json* file in the *src* folder (This file is shown below) by changing the value of the *phase* field in the *add_info* dictionary to match the name of your sequence. 

![Phase Unwrapping json file](/home/stluc/Pictures/BMAT_Pictures_vf/ph_un_json.png)

**This pipeline takes about 3 minutes per subject**
