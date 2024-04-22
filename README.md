# Ferlo EO Deep Learning Computer Vision for Forest Application 

![FERLO FOREST VISION](https://github.com/mmbaye/Counting-tree/blob/main/images/FerloForestVision.jpeg)

# Forest importance
Forests play a critical role in the global carbon cycle, as they absorb and store carbon dioxide $CO_2$ from the atmosphere through the process of photosynthesis. This process helps to mitigate the effects of increasing atmospheric $CO_2$  concentrations, which are a major contributor to climate change. Trees are important for carbon sequestration, as they can sequester large amounts of carbon in their wood, leaves, and roots. The amount of carbon that a tree can sequester depends on its size, species, and age, as well as the availability of water and nutrients. Large, mature trees are generally more efficient at sequestering carbon than younger trees, and some species of trees are more effective at sequestering carbon than others. For example, old-growth forests, which are composed of mature trees that have been growing for many years, can sequester large amounts of carbon in their biomass. In addition to sequestering carbon in their biomass, forests also help to reduce atmospheric $CO_2$  concentrations through the process of respiration, in which they release $CO_2$ back into the atmosphere. However, the net effect of forests on atmospheric $CO_2$  concentrations is still positive, as they absorb more $CO_2$ through photosynthesis than they release through respiration. Overall, forests play a vital role in mitigating climate change by sequestering carbon and reducing atmospheric $CO_2$  concentrations. Protecting and restoring forests is an important strategy for addressing the impacts of climate change.

# Context
In this project, we aim to construct a cutting-edge geospatial computer vision pipeline that will facilitate the identification of individual trees. Furthermore, we will develop an open-source package employing state-of-the-art deep learning models. Our initial focus will be on utilizing the data gathered for the Dundi Ferlo project in collaboration with CNRF/ISRA. Additionally, we will incorporate findings from the Foret classée de Mbow project, which shared a similar objective but primarily concentrated on leveraging high-resolution satellite data.

# Methodology 

![](https://github.com/mmbaye/Counting-tree/blob/main/images/methodology.jpg)

 1. Data Collection
  a. Satellite Imagery Acquisition
-  Objective: Obtain high-resolution satellite images that cover the targeted forest areas.
-  Action Steps :
  - Select open-source satellite data repositories.
  - Choose images with high spatial resolution (preferably under 1 meter) for better tree canopy differentiation.

  b. Drone Imagery Acquisition
-  Objective : Capture detailed aerial photographs and videos of the forest.
-  Action Steps :
  - Deploy drones equipped with high-resolution  RGB cameras 
  - Plan flight paths to ensure complete coverage and optimal lighting conditions for image quality.

 2. Image Preprocessing
  a. Image Correction and Enhancement
-  Objective : Improve the quality of raw images for better analysis.
-  Action Steps :
  - Apply radiometric and geometric corrections.
  - Enhance images using techniques such as histogram equalization or contrast adjustment.

  b. Image Registration
-  Objective : Align drone and satellite images to a common coordinate system.
-  Action Steps :
  - Use ground control points and GPS data for accurate image registration.
  - Employ software tools for automated alignment and calibration.

 3. Tree Detection Algorithm Development
  a. Feature Selection
-  Objective : Identify and select features significant for tree detection.
-  Action Steps :
  - Analyze textural, spectral, and spatial information relevant to tree species and canopy structure.
  - Use machine learning algorithms to identify the most discriminative features for tree detection.

  b. Model Training
-  Objective : Develop a robust computer vision model to detect individual trees.
-  Action Steps :
  - Collect training data from annotated images where individual trees are marked.
  - Choose a suitable machine learning or deep learning framework (e.g., SAM  and YOLO)

    ![](https://github.com/mmbaye/Counting-tree/blob/main/training%20/val_batch0_pred.jpg)


- Train the model using the selected features with cross-validation to ensure model accuracy.

 4. Tree Detection Implementation
  a. Running Detection Algorithms
-  Objective : Apply the trained model to new images for tree detection.
-  Action Steps :
  - Process the preprocessed images using the trained model.
  - Use sliding window techniques or region proposal algorithms to locate trees in the images.

  b. Validation and Accuracy Assessment
-  Objective : Evaluate the effectiveness and accuracy of the tree detection method.
-  Action Steps :
  - Compare detected tree locations with ground-truth data from field surveys.
  - Calculate metrics such as precision, recall, and F1-score to assess performance.

 5. Integration and Scaling
  a. Integration with GIS Systems
-  Objective : Integrate detected tree data into Geographic Information Systems (GIS) for further analysis.
-  Action Steps :
  - Convert detected tree coordinates into GIS-compatible formats.
  - Link tree data with other ecological or geographical datasets for comprehensive analysis.

  b. Scaling and Automation
-  Objective : Automate the process and scale up to cover larger areas.
-  Action Steps :
  - Develop scripts or applications that automate the workflow from image acquisition to tree detection.
  - Expand the model application to new areas using transfer learning techniques where applicable.
![image](https://github.com/mmbaye/Counting-tree/assets/10470281/64e31285-164e-4f18-8222-54a861c88b03)

