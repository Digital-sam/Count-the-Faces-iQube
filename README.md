# Count-the-Faces
C++ implementation of a "count face" script that counts the faces in an input picture array using the multilayer perceptron
# Approach
<ul>
  <li>resize each image</li>
  <li>load strings of weight and biases</li>
  <li>design a multilayer perceptor</li>
</ul>

## Code structure
#### define characters 
Get character from stdin. Returns the next character from the standard input (stdin)
```
define getchar
``` 
#### get and resizes the input dimension
```
struct Mat1d
``` 
#### declare weight and biases(as a string)
```
stringa0, stringa1
``` 
#### iterate through the string and return a vector
```
template<class T> vector<T> split_number(string in)
``` 
#### Initializes a new instance of the Array2D
```
struct Array2d {
``` 
#### Resize the dimension and transfer the generated 2D array to an external array
```
struct Transfer {
    Array2d W;
``` 
#### initialize softmax classifier
```
softmax(Array2d& dst, const Array2d& src) 
``` 
#### structure the multi layer perceptron; two hidden layers is developed
```
struct MLP {
    double eta;
``` 
#### Initializes a new instance of the Array2D
```
struct Array2d {
```
#### define the color structure as the tunning parameters
```
hueMin, hueMax, satMin, satMax, rThresh, grayThresh
``` 
#### structure the constant values, allocate and read
# References
Joint Face Detection and Alignment using Multi-task Cascaded Convolutional Networks
<ul><li>Kaipeng Zhang, Zhanpeng Zhang, Zhifeng Li, Yu Qiao</li></ul>
Deep Learning with Cpp
<ul><li>https://laptrinhx.com/deep-neural-network-from-scratch-in-c-for-learning-purposes-1380712153/</li></ul>
Navnit Kumar - 23/02/2021
