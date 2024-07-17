# Use-a-Pre-trained-Image-Classifier-to-Identify-Dog-Breeds

Program Instructions
To run the program, execute check_images.py in a terminal, providing up to three arguments. If any arguments are missing, default values are used.

Command Line Arguments:

Image Folder: Use --dir with a default value of 'pet_images'.
CNN Model Architecture: Use --arch with a default value of 'vgg' (options: 'vgg', 'alexnet', 'resnet').
Dog Names File: Use --dogfile with a default value of 'dognames.txt'.

To run all three models, you can use the provided bash scripts:

run_models_batch.sh: Executes all three models on local images and outputs results to a .txt file.
run_models_batch_uploaded.sh: Executes all three models on uploaded images and outputs results to a .txt file.

Program Outline:

1. Timing the Program:
  - Use the Time module to measure runtime.
     
2. Getting User Inputs:
  - Retrieve user inputs via command line arguments.
    
3. Creating Pet Image Labels:
  - Generate labels from pet image filenames and store them in a dictionary.
     
4. Generating and Comparing Classifier Labels:
  - Use the classifier function to create labels.
  - Compare these with pet image labels.
  - Store the results in a dictionary of lists.
    
5. Classifying as "Dogs" or "Not Dogs":
  - Classify labels using dognames.txt.
  - Update the dictionary with these classifications.
    
6. Calculating and Printing Results:
  - Determine the classifier's performance.
  - Print the results accordingly.
