# oneAPI Intel® 
Intel OneAPI serves as a comprehensive solution for heterogeneous application development, offering developers the flexibility, performance, and ease of use required to take full advantage of the increasingly diverse computing landscape. It enables developers to write high-performance code that can seamlessly target multiple hardware architectures, accelerating the pace of innovation and unlocking new possibilities in the field of computing.
OneAPI offers a unified programming model that allows developers to write code that can seamlessly target various computing devices, including CPUs, GPUs, FPGAs, and other accelerators. This eliminates the need for separate code bases for different hardware architectures, simplifying the development process and reducing maintenance efforts.

## Adantages of using oneDAL and oneDNN 
Using both oneDAL (Intel Data Analytics Library) and oneDNN (Deep Neural Network Library) models together provides several advantages:

1. **Performance Optimization**: Both oneDAL and oneDNN are optimized libraries that leverage Intel processors and architectures to deliver high-performance computations. They are designed to efficiently utilize the available hardware resources, such as multi-core processors, vector instructions (e.g., Intel Advanced Vector Extensions - AVX), and specialized acceleration features (e.g., Intel Deep Learning Boost - DL Boost). By utilizing these optimizations, oneDAL and oneDNN models can achieve faster execution times and improved overall performance, enabling efficient data analytics and deep learning tasks.

2. **Versatility**: oneDAL covers a wide range of data analytics tasks, including machine learning, data preprocessing, and mathematical computations. On the other hand, oneDNN focuses on deep neural networks and provides optimized primitives for deep learning operations, such as convolutions, pooling, and activation functions. By combining the two libraries, you gain versatility in tackling both traditional data analytics tasks and deep learning tasks within a unified framework.

3. **Seamless Integration**: oneDAL and oneDNN can be seamlessly integrated with popular programming languages and frameworks. oneDAL supports integration with Python and popular data science frameworks like scikit-learn and NumPy. Similarly, oneDNN integrates well with deep learning frameworks such as TensorFlow and PyTorch. This integration allows you to leverage the capabilities of oneDAL and oneDNN while benefiting from the familiar APIs and ecosystems of these frameworks, simplifying the development process and enabling efficient utilization of the libraries' functionality.

4. **Cross-Platform Compatibility**: Both oneDAL and oneDNN are designed to be cross-platform compatible, enabling you to develop applications that can run on various operating systems, including Windows, Linux, and macOS. This flexibility ensures compatibility and ease of use across different platforms, allowing you to deploy your models in diverse environments without major modifications.

5. **Scalability**: oneDAL and oneDNN models are built with scalability in mind. They provide efficient parallel processing capabilities, allowing you to distribute computations across multiple cores or even across distributed computing environments. This scalability enables you to handle large datasets, perform efficient model training, and process high-volume data in a timely manner.

6. **Intel Hardware Optimizations**: Intel processors offer advanced hardware features that can accelerate data analytics and deep learning tasks. Both oneDAL and oneDNN take advantage of these hardware optimizations, such as AVX instructions and DL Boost. Leveraging these features can significantly boost performance, providing faster execution and reducing training and inference times.

In summary, utilizing both oneDAL and oneDNN models provides advantages in terms of performance optimization, versatility, seamless integration with popular frameworks, cross-platform compatibility, scalability, and leveraging Intel hardware optimizations. This combination empowers developers and data scientists to efficiently tackle a wide range of data analytics and deep learning tasks while harnessing the power of Intel's hardware architectures.

### Project 1: Heart Disease Prediction 

To develop a heart disease prediction model, these algorithms are trained on labeled datasets containing patient data and corresponding heart disease labels. The dataset is divided into training and testing sets, and the algorithm is trained on the training set to learn patterns and relationships. The model's performance is then evaluated on the testing set to assess its predictive accuracy.
1. **Logistic Regression**: This algorithm is often used for binary classification problems, making it suitable for predicting the presence or absence of heart disease based on patient features. Logistic regression models estimate the probability of a patient having heart disease based on the input variables.
2. **Decsion Tree**: Decsion tree is an ensemble learning algorithm, It can handle complex relationships between variables and can provide feature importance rankings, helping identify which factors contribute most to heart disease risk.

In this project we have used **sciket learn extended by Intel to split the test and train data.
<img width="992" alt="Screenshot 2023-05-17 at 10 04 53 AM" src="https://github.com/Ragzoid/oneAPI-Intel-/assets/90862154/3fa9fe7c-b7f6-47da-90e7-5c1db90cceb1">

Further, we have used Logistic Regresession and Decision Tree models to test the accuracy of the models.
<img width="995" alt="Screenshot 2023-05-17 at 10 07 05 AM" src="https://github.com/Ragzoid/oneAPI-Intel-/assets/90862154/f1552766-45c7-435b-8e72-00768efdf5be">

We provided a comparitive analysis between normal sciket learn model and the model extended by oneAPI Intel®. There is not huge difference in terms of execution time of the models when the dataset size is low, wheras when tested with large dateset **oneDAL** performed 10x times better.
