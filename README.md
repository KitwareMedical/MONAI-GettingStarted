# MONAI-GettingStarted

## Why MONAI?

MONAI began as a collaboration between KCL and Nvidia but rapidly expanded to include a massive community of highly skilled and very dedicated researchers and developers from around the world. Why was this adoption so quick? Because MONAI addresses the specific needs and opportunities of deep learning in medical imaging:

* Medical Image Data: MONAI supports a variety of medical image formats (thanks to ITK, GDCM, NIBabble, and other toolkits), and it respects the physical properties of those images, e.g., pixel size, pixel spacing, and image orientation. Those physical properties are often ignored by traditional computer vision libraries, but they are essential to the accurate and real-world application of deep learning to clinical medical images.
* Medical Image Transforms: MONAI includes a multitude of domain-specific transforms for medical image pre-processing and augmentation. Unlike with photographs or other common computer vision data, it is often not appropriate to rotate, flip, or change the intensities (e.g., Hounsfield Units) of medical images for augmentation purposes, yet warping the anatomy in images to match patient variations, removing ribs from x-ray images, and other steps are common in medical image pipelines and are provide by MONAI via ITK, DKFZ’s BatchGenerator, ICL’s DLTK, KCL’s NiftyNet, and other transform libraries that have been integrated into MONAI.
* Medical Workflows: 3D Slicer provides a user-friendly interface for applying trained MONAI models to clinical workflows for a variety of disease diagnosis, treatment planning, and treatment guidance research. Similarly, AWS’s SageMaker, Google’s CoLab, and Nvidia’s Clara provide cloud-based platforms for hosting MONAI research, development, and deployment platforms. Efforts to integrate MONAI inference capabilities with easy-to-deploy web-based 3D radiological viewers such as ParaViewMedical are also underway.
* Reproducibility and Standardization: Underlying the design and implementation of MONAI is a commitment to promote reproducibility and build upon existing standards. Reproducibility is paramount to clinical deep learning regulatory documentation, validation, and acceptance. MONAI carefully documents its operating environment, I/O methods, random seeds, data sources, and more to aid in these reproducibility efforts. Similarly, rather than forming an alternative to PyTorch, MONAI builds upon and maintains compatibility with PyTorch. Rather than creating its own I/O system, it uses ITK. Rather than implementing every data transform from scratch, it uses libraries from DKFZ, KCL, ICL, ITK, and others. Communities are coming together, rather than competing, and the power of open source is growing more rapidly as a result.
* Interactive Visualization and Best Practices: MONAI comes bundled with multiple Jupyter Notebooks that exemplify best practices for deep learning in medical imaging. These notebooks explore common tasks and replicate results from top performing networks in several medical imaging grand challenges. Furthermore, we have paired MONAI with ITKWidgets that bring interactive visualization and annotation capabilities to Jupyter Labs and Notebooks. ITKWidgets enable deep learning inputs, intermediate values, and results to be visualized, explored, and optionally refined by researchers and clinical collaborators with ease. Such interactive visualization of inputs and intermediate results are crucial to avoid hours and days of wasted training time and to gain new insights into results.

## Introductory Slides and Videos

We have also work with other members of the MONAI team to develop three sets of slides that are targeted for different audiences. These slides do provide some guidance on their own, but they are really meant to be used by lecturers who already know MONAI and who want to introduce MONAI to others.

1. MONAI: A three minute introduction:
https://www2.slideshare.net/StephenAylward1/monai-medical-image-deep-learning-a-3-minute-introduction
These slides were presented at the start of the 2020 3D Slicer Project Week. A video recording of that presentation is given here. Admittedly, the video contains some references specific to that venue, but the overall message is general and should help guide the use of the 3-minute introductory slides.
https://www.youtube.com/watch?v=tBrMVTlzb8s

2. MONAI for Data Scientists and Developers:
https://www2.slideshare.net/StephenAylward1/monai-medical-imaging-ai-for-data-scientists-and-developers-3d-slicer-project-week-2020
These slides were part of an hour long presentation on MONAI given during the 2020 3D Slicer Project Week. This presentation is geared towards Pytorch / Python users, deep learning researchers, and data scientists who would like an overview of why MONAI should be used for medical imaging deep learning research and application development.

3. MONAI and Open Science for Clinicians and Project Managers:
https://www2.slideshare.net/StephenAylward1/monai-and-open-science-for-medical-imaging-deep-learning-sipaim-2020
These slides were given as a keynote presentation at the 16th International Symposium on Medical Information Processing and Analysis (SIPAIM 2020). These slides promote open science practices, acknowledge open science as a major reason for the success of deep learning, and introduce MONAI as an open science platform. A recording of the keynote presentation is also available online:
https://youtu.be/XHJcKheftrc

# Additional MONAI Material and Forums

* Getting Started as a MONAI User:
    * https://monai.io/start.html
* Getting Started as a MONAI Developer:
    * Community Guide:
        * https://github.com/Project-MONAI/MONAI#community
    * Contributing Guide:
        * https://github.com/Project-MONAI/MONAI#contributing
    * Suggestions for first contributions:
        * Look for the “Good First Issue” tag on the MONAI issue tracker: https://github.com/Project-MONAI/MONAI/labels/good%20first%20issue
* Q&A forums:
    * PyTorch Forums. Tag @monai or see the MONAI user page.
        * https://discuss.pytorch.org/u/MONAI/
    * Stack Overflow:
        * https://stackoverflow.com/questions/tagged/monai
    * To join the MONAI Slack Channel, please fill out the Google form:
        * https://forms.gle/QTxJq3hFictp31UM9
* MONAI News:
    * https://www.linkedin.com/search/results/content/?keywords=MONAI
    * https://twitter.com/ProjectMONAI
