# pipegan
1.  Load datasetPipe folder to your data repository
2.  Load pipecyclegan.ipynb notebook in Colab to:
    a.  Train the CycleGAN model for damage spread (referencing datasetPipe in item #1)
    b.  Convert the CycleGAN model to TFLite for deployment to an edge device
3.  Load and execute gan project file locally.  With the edge device connected (i.e. Coral USB Accelerator), execute pipe_gan.py to run inference using the edge device.
Shell command:
python3 pipe_gan.py \
  --model models/pipegan.tflite \
  --input images/good13.jpeg
