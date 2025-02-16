# DiaOutline: Contour Extraction for Morphometric Analysis

Contacts:
Niksoney Azevedo Mendonça/UFPE - Master in Plant Biology, currently a PhD student in the same program <br>
Email: niksoneyazevedo2017@gmail.com <br>
WhatsApp: https://wa.me/55989912136367text= <br>

Welcome to the DiaOutline repository, a powerful and intuitive tool for extracting contours from images, specially designed for morphometric studies in plant biology and related areas. This software, developed by Wishkerman & Hamilton (2018), uses advanced image processing techniques and Fourier analysis to extract precise contours of objects, such as leaves, fronds and other biological structures.

Here, you will find a detailed step-by-step guide to installing and using DiaOutline, from setting up the environment to extracting and exporting data for statistical analysis. In addition, we provide download links for the necessary versions of the software and practical tips to optimize the processing of your images.

Whether you are a researcher, student or enthusiast of plant biology, this repository was created to facilitate your work with shape and contour analysis, allowing you to focus on what really matters: science!

What you will find here:

1. Detailed instructions for installing Matlab Runtime and DiaOutline.
2. A step-by-step guide to image processing and contour extraction.
3. Tips for preparing images and optimizing results.
4. Links to download the programs.

Feel free to explore, contribute and use this material in your research. If you have any questions or suggestions, do not hesitate to contact us!

Let's explore the world of shapes and contours together? 🌿✨

## Let's get started

#Step 1 - Install Matlab!

Download and install Matlab Runtime 9.3 (only this version works):
http://www.mathworks.com/products/compiler/mcr/index.html

#Step 2 - Install DiaOutline

Download and install DiaOutline:
https://github.com/wishkerman/DiaOutline (follow the instructions here)

If you prefer, I have the Matlab and DiaOutline versions on my OneDrive for installation:
Matlab is on the first page when you open the link, and DiaOutline is located at: DiaOutline-master -> Application -> DiaOutlineV101 (remember to download the entire folder and unzip it on your computer).
[https://1drv.ms/f/slAtpCyyNefO09gdBDG-Nfu6We_T3ajQ?e=3OLUIj](https://1drv.ms/f/s!AtpCyvNefO09gdBDG-Nfu6We_T3ajQ?e=ld3XSH)

Note: To proceed to Step 3, you must have images in (preferably) .png format, and the images should have a clean background so that the Fourier coordinates are extracted exclusively from the images of interest and not from other artifacts. Remember that when mounting boards, it is interesting to make one per exsiccate.

Suggested applications:
Gimp: https://www.gimp.org/ or Photoshop (paid version)

#Step 3 - Use DiaOutline to extract outlines
After processing the images and isolating the fronds of interest, you will be ready to use DiaOutline.
![Captura de tela 2025-02-16 125932](https://github.com/user-attachments/assets/86166440-f378-41fb-bdb0-a2a29911508c)

Step-by-step instructions:

1. Select working folder – In this option, you will define your directory, i.e., the folder where all the images are located (you won’t see any images here, so don’t worry).

2. Load image – Here you will select an image to start the process. Keep in mind that this process can take some time because it processes one board at a time.

3. Change contrast – Adjust the contrast of the image to improve the visibility of the fronds and outlines.

4. Threshold image – Apply thresholding to separate the objects of interest from the background. This will create a binary image where the outlines of the fronds will be easier to identify.

5. Invert image – Invert the binary image if necessary to ensure that the fronds are highlighted in white on a black background.

6. Fill image – Fill in any internal holes in the fronds, ensuring that the object is solid and without flaws before proceeding.

7. Max. value (pixel) for removal – Set the maximum pixel value for the removal of small objects or noise that are not of interest.

8. Remove small objects – Remove small objects or artifacts that may be present in the image, leaving only the fronds of interest.

9. Trace outline – Start the process of tracing the outlines of the fronds. This step will extract the precise outlines of the fronds, which will be used for further analysis.

10. Save file name pattern – Here you will define the name of the image (don’t worry, you can update the name later in step 15).

11. Generate data – Generate the outline data, such as the coordinates of the points, which can be exported for further analysis in R.

12. Save data – Your data will be saved in .TXT format for use in other tools or statistical analyses.

13. Visualization in the environment – In this environment, you will visualize the images of the board from which you are extracting the outlines. In the example, there are two leaves and two numbers, 1 and 2, which means that it extracted two different shapes from this image.

14. Data visualization – In this step, you will have three columns with information. Column 1: the number of the outline visualized in step 14. Column 2: the values corresponding to the outline of each image; these are the values we will use in R for analysis. Column 3: the name of the species you defined in step 11, remembering that you can change the name here.

15. Save Image (TIFF or PNG) – Here you can save the exact image you are visualizing in the interface from step 14 (note that it is only useful for visualization and is not necessary for the images).

16. Quit – Here you finish and close the program.

REFERENCE
Wishkerman, A., & Hamilton, P. B. (2018). Shape outline extraction software (DiaOutline) for elliptic Fourier analysis application in morphometric studies. Applications in Plant Sciences, 6(12), e01204.
