# JPG to HDRI Converter

This repository contains a machine learning model designed to convert 8-bit JPG images to 16-bit High Dynamic Range Images (HDRI). The model is currently at an early training stage and is expected to improve over time.

## Prerequisites

Before you begin, ensure you have the following required files:

- **Model Weights**: Located in the `checkpoint` folder, these are essential for the model to function correctly.
- **jpg_to_hdri Group**: This is a crucial component of the process that converts the source image to a logarithmic color space before the model attempts to determine pixels that could be clamped in an 8-bit image.

## Setup

1. Clone this repository to your local machine using `git clone`.
2. Ensure that the `checkpoint` folder is placed in the root directory of the cloned repository. If you move the .cat file, make sure to point to it using the group's model file knob.
3. Try out the example jpg included from Poly Haven or plug in your own to try out.


## Limitations

- The model is in the early stages of training and is subject to improvements.
- Model has been only trained on Latlong hdris,
its effect on rectilenear images is unknown!
- There might be performance issues with images over 4K resolution. Tests conducted on an M1 Mac have indicated limitations with high-resolution images.

## Contributions

Contributions to improve the model are welcome. Please submit a pull request or open an issue if you have suggestions or contributions.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Aknowledgements

Poly Haven for the test hdris and The Foundry for its amazing CopyCat tool. 