# breast-cancer-image-segmentation



## Runnable scripts/commands: what are the main commands that you run to get the results
- For the dataset:

    wget https://zenodo.org/record/1175282/files/TNBC_NucleiSegmentation.zip -O dataset.zip
    unzip dataset.zip
    
- To run UNET, eNET, or MLP Models:
    
    `python3 train.py`
    
- To run FCN Model (with original data):
    
    `python3 fcn_train_no_aug.py`
    
- To run FCN Model (with augmented data):
    
    `python3 fcn_train_aug.py`
    
    - To run different fcn resnet models, just have to change the model assigned on line 39, can uncomment the desired model

- To run notebooks in augmentation_validation/, open the notebook of interest in Colab, change the wandb login to your own (or comment out all wandb lines) if running a training notebook, and run the notebook.
    - To run the augmentation_validation.ipynb notebook, you will also need to place the model weights into your own Google Drive (find the link to the weights in best_weights_augVal/README.md) and, in the notebook, accordingly set the path pointing to the weights.

