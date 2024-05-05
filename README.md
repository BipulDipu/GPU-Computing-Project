```markdown
# BM40A1401 GPU Computing Project Report

## Date: 02/04/2024

Students:
- Bipul Biswas, 000359670 (Leading role in KNN Code and report)
- Usama Nasrullah, 000974615 (Leading role in MLP Code and report and overall we shared the whole work)

## Abstract
This comprehensive report covers the acceleration of machine learning algorithms through the implementation of Graphics Processing Units. We examined two algorithms, k-Nearest Neighbors and Multilayer Perceptron, and presented how this acceleration plays out. We conducted a series of experiments to determine the values of execution time, training duration, inference speed, and the associated accuracies across each of the models. Our experimental insights have shown the possibility and desirability of machine learning with GPU acceleration. Moreover, it influences the necessary compromise between faster computing speeds and model accuracy.

## Introduction
kNN is simple and MLP is basic for the deeper version of neural networks, both approaches become challenging with large or high-dimension datasets. Therefore, the primary goal of the research is to apply GPU computing to various computational tasks of these algorithms to make them more practical and efficient.

## Methodology
### Data Preparation
The data set consists of 4,000 observations and 10 numerical features. The observations represent 10 classes and the class labels are given as numbers in the last column of the file making the total number of columns 11. For both kNN and MLP approaches, we ensured standard data preprocessing practices including data normalization to facilitate efficient training.

### KNN Implementation
In order to exploit the computational capabilities of GPUs for the k-Nearest Neighbors algorithm, a custom implementation was developed, utilizing the CUDA toolkit through CuPy’s RawKernel. More specifically, the goal of this method was to improve the efficiency of the distance computation function which is one of the primary computational bottlenecks of the kNN algorithm particularly when dealing with large datasets and high-dimensional spaces.

### MLP Implementation
To demonstrate the Impact of GPU in calculations of the MLP learning process in our work shows us the practical advantages and techniques leveraging GPU acceleration in machine learning. This part precisely introduces our MLP model's architecture and training processes, where we emphasize on the significant evaluation metrics which were diligently noted as we ran the experiments both on the CPU and GPU systems.

## Results
### KNN Performance Analysis
On the acceleration capabilities of GPU computing, the performance of the kNN model was also keenly evaluated, offering key understandings over the dynamics of the execution time and classification accuracy.

### MLP Performance Analysis
For proper learning, the MLP model was trained for 100 epochs. The Adam optimizer was used to find a balance between flexibility and robustness; the learning rate was set to 0.001. The CrossEntropyLoss was used to help the model predict more effectively – this function measures the scoring rule of the discrepancy between the predicted probabilities and the actual multiclass labels.

## Discussion
Experiments demonstrate the potential of the GPU acceleration in the improvement of machine learning computations. Although the kNN model indicates the significance of the ‘k’ parameter in achieving ideal accuracy, the MLP model fails to show the impact of hardware choice on model accuracy, despite the significant reduction in inference time when using the GPU.

## Conclusion
Our exploration regarding k-nearest neighbors and multilayer perceptron models in machine learning using GPU acceleration demonstrated how innovative hardware can change and refine the concept of all proportional factors. Obviously, both models demonstrated high effectiveness, yet we have also realized that the maximum benefit could be derived only under certain conditions.
```
