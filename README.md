# Neural Network Implementation

## Description
This repository provides a straightforward implementation of a feedforward neural network in C++. It leverages Eigen for matrix computations and Boost for initializing weights and biases with random values. It's designed to be an educational resource for understanding the basics of neural networks, including training and prediction processes.

## Prerequisites
- C++ Compiler (C++11 or above)
- Eigen Library
- Boost Library
- matplotlibcpp (matplotlib for C++)

## File Structure
- `network.cpp`: Contains the entire neural network implementation and execution.
- `mnist_train.csv`: Example training data file (not included in this repository).
- `mnist_test.csv`: Example testing data file (not included in this repository).

## Compilation and Execution
1. Ensure all prerequisites are installed and accessible in your build environment.
2. Compile the program with appropriate include paths for the Eigen and Boost libraries. If you're using g++, the command might look like this:

    ```
    g++ -std=c++11 -I /path/to/Eigen -I /path/to/Boost main.cpp -o neural_network
    ```

3. Run the compiled executable:

    ```
    ./neural_network
    ```

## Implementation Details
- The `Layer` class represents a layer in the neural network, handling forward propagation.
- The `ActivationFunc` class encapsulates activation functions and their derivatives.
- The `Network` class manages layers, forward and backward propagation, and training over epochs.
- Random weight initialization is performed using Boost's random number generation.
- The network is tested with MNIST dataset in the provided example.

## Contributing
- For major changes, please open an issue first to discuss what you would like to change.
- Ensure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
