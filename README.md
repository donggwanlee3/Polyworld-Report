# Technical Assessment for Machine Learning Engineer Internship

## Project Overview
This technical assessment focuses on implementing and extending the PolyWorld algorithm, which is designed for extracting building polygons from satellite imagery. The project is structured into three progressive levels, each building on the previous one, and is intended to evaluate your ability to implement existing research, improve upon it, and solve real-world problems in innovative ways.

## Data
The dataset for this project consists of two parts: 
1. The Polyworld paper (https://arxiv.org/abs/2111.15491) and github repository (https://github.com/zorzi-s/PolyWorldPretrainedNetwork). The repository includes all the informatino you need to access their code, instructions for implementation and image data.

2. High-resolution satellite images from BlackPrint Technologies. We will let the candidate decide which images to use for the test. The images can be found in the following drive link: https://drive.google.com/drive/folders/19UqNC3R7DGIIbqGxR8XZ2OBzkbrYxhs6?usp=sharing 

## Levels of Difficulty

### Level 1: Reproducing Existing Results

**Objective:** Clone the existing GitHub repository of the PolyWorld paper and reproduce the results using the provided images in the repository.
**Tasks:**
- Clone the PolyWorld GitHub repository and set up the environment to run the model as per the instructions provided.
- Run the model on the original dataset provided in the PolyWorld repository to reproduce the results.
- Write a critique of the results, discussing the model’s performance, potential limitations, and areas for improvement.

**Deliverables:**
- A report that includes your critique of the model along with suggestions for future improvements.
- Evidence of the reproduced results (screenshots, output files) and code used.

### Level 2: Adapting the Model to New Images

**Objective:** Apply the PolyWorld model to a new set of images provided by BlackPrint, which will likely require additional preprocessing techniques.

**Tasks:**
- Preprocess the new images to fit the input requirements of the PolyWorld model. This may include image resizing, normalization, or other image enhancement techniques to improve model performance.
- Run the PolyWorld model on these preprocessed images and analyze the results.

**Deliverables:**
- A detailed description of the preprocessing steps you implemented.
- A comparison of results between the original and new images.
- Visuals and output data demonstrating the model's performance on the new images.
- All of the code used. 

### Level 3: Solving the Patching Problem

**Objective:** As images need to be cropped before they are processed, many buildings en up being cut which produces many inaccuracies in the restitching part of the process. Propose and, if possible, implement a solution to address thus issue of inaccuracies caused by the image patching process used in the model.  

**Tasks:**
- Research and propose a technique to improve how the model handles the cropping of large images into smaller chunks, focusing on minimizing errors when these chunks are reassembled and buildings that have been cropped are stitched back together. 
- Discuss the efficiency and feasibility of your proposed solution.
- For extra credit, implement this technique within the pipeline and showcase the improved results (if successful you are guaranteed a position at BlackPrint)

**Deliverables:**
- A report detailing your proposed solution, its theoretical basis, and expected benefits.
- If implemented, provide code modifications, a demonstration of the solution in action, and a before-and-after comparison.

## Submission Guidelines
Submit your work through this private GitHub repository. Work in your own branch and create a pull request when done with this assessment. 
Include a README file in your repository that provides:
- An overview of your solution.
- Instructions on how to set up and run your code.
- A discussion of any challenges you faced and how you addressed them.
- Ensure your code is well-commented and organized.

## Evaluation Criteria
- **Accuracy and Quality of Implementation:** How well does your solution align with the PolyWorld model's standards and improve upon them?
- **Innovation and Problem Solving:** How effectively do you address and propose solutions to the identified problems?
- **Code Quality:** Is your code clean, organized, and well-documented?
- **Completeness of Deliverables:** Have you met all the deliverables for the level you chose to complete, particularly in proposing and potentially solving the proposed problem?