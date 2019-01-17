# DogImageClassifier
A dog breed classifier that uses a provided CNN architecture to identify dog breeds

# Usage 
Command to execute classifier: </br>
```python check_images.py --dir \<directory with images> --arch \<model> --dogfile \<file that contains dognames>```

Batch execution: </br> 
```sh run_models_batch.sh```

# Results
| Total images | Dog images | Other images |
| ------------ | ---------- | ------------ |
| 40 | 30 | 10 |
  
| Architecture | % Not-a-dog correct | % Dogs correct | % Breeds correct | % File & classifier labels match |
| --- | --- | ---| --- | --- |
| ResNet | 90.0% | 100.0% | 90.0% | 82.5%
| AlexNet | 100.0% | 100.0% | 80.0% | 75.0% 
| VGG | **100.0%** | **100.0%** | **93.3%** | **87.5%**

Based on these results and the set of classified images, the best model architecture is VGG.
