# Braille Decoding Algorithm

This repository contains an algorithm implemented in Python for decoding Braille characters from an input image. The algorithm traverses a 3x2 Braille matrix, detects the dots present, and maps them to corresponding characters based on their positions. The aim of this project is to provide a reliable and efficient method for decoding Braille characters from digital images.

## Algorithm Overview

1. The input image is read using the OpenCV library and converted to a binary image with two values: 0 (black) and 255 (white).
2. The algorithm performs 8-connectivity analysis on the binary image to identify individual Braille dots and assigns labels to them.
3. Labels are updated based on equivalency lists to ensure consistency.
4. The center points of all the dots are calculated to determine the shortest distance between two dots.
5. The algorithm traverses the image pixel by pixel, decodes the Braille characters using clockwise and anticlockwise traversal, and generates the final output string.
6. Spaces are added between words based on the distance between dots.
7. The decoded output is printed on the console and saved in a text file named "Algorithm Output".

## Results

The algorithm successfully decodes Braille characters from the input image and provides the corresponding text output. The output is both printed on the console and saved in a text file for further analysis or usage. The algorithm demonstrates efficient Braille decoding capabilities and can be used for various applications involving Braille text recognition.

Please note that the algorithm assumes the input image follows the standard Braille dot arrangement and may not be suitable for non-standard layouts or variations in Braille representation.

## Usage

To use the algorithm, follow these steps:

1. Clone the repository to your local machine.
2. Install the required dependencies, including NumPy and OpenCV.
3. Provide the input image named "Braille.png" in the root directory of the repository.
4. Run the Python script, and the decoded output will be printed on the console and saved in a file named "Algorithm Output".

Feel free to modify the code or integrate it into your own projects as needed.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code for personal or commercial purposes.
