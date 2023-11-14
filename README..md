# MNIST Keras Model on STM32 with CubeMX and CubeAI

This is a README file that provides instructions for using the MNIST Keras model on an STM32 microcontroller using CubeMX and CubeAI.

## Overview

The MNIST dataset is a popular dataset used for training and testing machine learning models. It consists of a large set of handwritten digit images along with their corresponding labels. In this project, we will train a Keras model on the MNIST dataset and then deploy it on an STM32 microcontroller using CubeMX and CubeAI.

## Prerequisites

Before getting started, make sure you have the following:

1. STM32 microcontroller board: You will need an STM32 microcontroller board to run the model. Examples include STM32F4 Discovery, STM32F7 Discovery, or STM32H7 Discovery.

2. CubeMX: CubeMX is a graphical tool that allows you to configure STM32 microcontrollers and generate initialization code. You can download it from the STMicroelectronics website.

3. CubeAI: CubeAI is a software package provided by STMicroelectronics that enables running deep learning models on STM32 microcontrollers. It integrates with CubeMX to simplify the deployment process. You can download it from the STMicroelectronics website.

4. Python and TensorFlow: You will need Python and TensorFlow installed on your development machine to train the Keras model.

## Steps

Follow these steps to use the MNIST Keras model on an STM32 microcontroller:

1. **Prepare the Keras Model**: First, you need to train a Keras model on the MNIST dataset. There are many tutorials available online on how to train a simple MNIST model in Keras. Once you have trained the model, save it in the HDF5 format (`.h5`).

2. **Import the Model in CubeMX**: Open CubeMX and create a new project for your STM32 microcontroller. In the "Project Manager" tab, locate the "AI Validation" section and click on "Add" to import the Keras model file (`.h5`). CubeMX will convert the Keras model to a format compatible with the STM32 microcontroller.

3. **Generate Code**: After importing the Keras model, go to the "Project" tab in CubeMX and configure the project settings as needed. Then click on "Project" > "Generate Code" to generate the initialization code for your project.

4. **Compile and Flash**: Open the generated code in your preferred Integrated Development Environment (IDE) and build the project. Once the build is successful, connect your STM32 microcontroller board to your computer and flash the generated binary onto the board.

5. **Run the Model**: After flashing the binary onto the board, you can run the model on the STM32 microcontroller. The model will take input from the onboard sensors or any other input source you have configured and provide the predicted digit output.

## Additional Resources

- [STMicroelectronics Website](https://www.st.com/): Visit the STMicroelectronics website for more information on STM32 microcontrollers, CubeMX, and CubeAI.

- [Keras Documentation](https://keras.io/): The official documentation for Keras provides detailed information on how to train and save models in Keras.

- [STM32Cube.AI Documentation](https://www.st.com/en/embedded-software/stm32cube-ai.html): The official documentation for STM32Cube.AI provides instructions and examples for using deep learning models on STM32 microcontrollers.

- Online tutorials and forums: There are many online tutorials and forums available where you can find step-by-step guides and solutions to common issues when working with CubeMX, CubeAI, and STM32 microcontrollers.

## Conclusion

Using CubeMX and CubeAI, you can easily deploy a trained Keras model on an STM32 microcontroller, enabling you to run machine learning algorithms directly on the microcontroller. This opens up possibilities for implementing intelligent applications in resource-constrained environments.