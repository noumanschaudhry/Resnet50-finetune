# Resnet50-finetune
finetune pretrained resnet50 on your own data.

This repo contains the code for the finetuning of pretrained ResNet50. ResNet50 is preloaded with trained weights of ImageNet, and you can further finetune that on your own data by follwing simple steps.
For to run this code your data should be in different folders namely Train and Val (Validation) each of which will have subsequent folders based on the number of classes. Lets say we have 2 classes so both Train and Val will have 2 subdirectories each.


For to make this even easier I have applied a data_split script, just include the data_split file and call createTrainValSplit(directory where data is ,how you want to split your data)
For example you want 20% validation and 80% train createTrainValSplit('folderA/data',0.2)
