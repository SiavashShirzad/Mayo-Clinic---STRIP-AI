# Mayo-Clinic---STRIP-AI
My solution for Mayo Clinic - STRIP AI Kaggle competition

## Data selection

As I coded in the preprocessing notebook, I selected the coordinations of 512x512 images containing histological data based on pixel data Standard Deviations for each Whole-Slide image and saved them in a CSV file.

## Model

As demonstrated in mayo-patho.ipynb the main model was based on EfficientNetB1 with 5 inputs. 5 inputs were randomely selected from coordination of a whole-slide image and the go through a single pretrained model (because I wanted to extract same features from each image). The after concatination and some layers the model returns a single neuron with sigmoid as activation function.
