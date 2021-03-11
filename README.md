# Color-Camera-ISP-Pipeline--Python

Program Management
We have received a large RAW image set from a customer. The Atlas team must process the RAWdataset to convert to RGB and pass the images to an data annotation team for for data labelling sothat they can be used by a computer vision team for neural network training.

* Briefly describe the project milestones or workflow you would set for the Atlas team tocoordinate with the other two teams and deliver timely and sucessfully on the project.
Programming assignment
The objective of this assignment is to propose an image processing pipeline to processcompanded HDR RAW images in either Python or C/C++. A set of such RAW images captured inchallenging conditions is included in images/

The RAW images have the following format:
BITDEPTH = 16 bits 
COLS = 2880 
ROWS = 1860 
HEADER_ROWS = 5 
TRAILER_ROWS = 6 CFA_ORDER = RGGB

Tasks:
1. Develop a function to open a companded RAW image from disk and return a linear RAWimage. In Python, you can use
numpy.fromfile and the linearize function providedbelow.
2. Implement a minimal image processing pipeline to convert the RAW images to RGB. Theimages are intended for annotation so scene objects must be clearly visible and identifiable.Objects or interest are pedestrains, cyclists, vehicles, traffic lights and road signs. Justify theorder of the blocks implemented and the algorithms used. You can use any available libraries.Make sure the pipeline can handle diverse capture conditions by testing it on the providedRAW images.
3. Display or store the processed RGB image to disk.
