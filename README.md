# Stats Strided MskMax 📊

![GitHub Release](https://img.shields.io/github/release/Korva44/stats-strided-mskmax.svg) ![License](https://img.shields.io/badge/license-MIT-blue.svg)

Welcome to the **Stats Strided MskMax** repository! This project allows you to calculate the maximum value of a strided array according to a mask. This functionality is essential for various mathematical and statistical operations where you want to focus on specific elements of an array while ignoring others.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

In many mathematical computations, you may need to find the maximum value of certain elements in an array. The **Stats Strided MskMax** library provides an efficient way to do this by using a mask. A mask is an array of boolean values that indicate which elements should be considered in the calculation.

This repository is designed for developers who need to perform statistical analysis on data sets while ignoring certain values. Whether you are working in data science, machine learning, or any field that requires statistical computations, this library will help you streamline your processes.

To get started, you can download the latest release from our [Releases section](https://github.com/Korva44/stats-strided-mskmax/releases). 

## Installation

To install the **Stats Strided MskMax** library, you can use npm. Open your terminal and run the following command:

```bash
npm install stats-strided-mskmax
```

This command will download the package and add it to your project. Make sure you have Node.js installed on your machine before running this command.

## Usage

Once you have installed the library, you can import it into your JavaScript file. Here’s a simple example of how to use the library:

```javascript
const mskmax = require('stats-strided-mskmax');

const array = [1, 2, 3, 4, 5];
const mask = [true, false, true, false, true];
const stride = 1;

const maxValue = mskmax(array, mask, stride);
console.log(maxValue); // Output: 5
```

In this example, the function will only consider the values at the indices where the mask is `true`, which are `1`, `3`, and `5`. The maximum of these values is `5`.

## API Documentation

### Function: `mskmax(array, mask, stride)`

- **Parameters:**
  - `array` (Array): The input array of numbers.
  - `mask` (Array): A boolean array that indicates which elements to consider.
  - `stride` (Number): The step size to take when traversing the array.

- **Returns:**
  - (Number): The maximum value found in the strided array according to the mask.

### Example

Here’s a more complex example:

```javascript
const array = [10, 20, 30, 40, 50];
const mask = [false, true, true, false, true];
const stride = 1;

const maxValue = mskmax(array, mask, stride);
console.log(maxValue); // Output: 50
```

In this case, the maximum value is `50`, which is the highest number among the elements where the mask is `true`.

## Examples

### Example 1: Basic Usage

```javascript
const array = [3, 1, 4, 1, 5, 9];
const mask = [true, false, true, false, true, false];
const stride = 1;

const maxValue = mskmax(array, mask, stride);
console.log(maxValue); // Output: 5
```

### Example 2: Using a Different Stride

```javascript
const array = [2, 7, 1, 8, 2, 8];
const mask = [true, true, false, true, false, true];
const stride = 2;

const maxValue = mskmax(array, mask, stride);
console.log(maxValue); // Output: 8
```

## Contributing

We welcome contributions to the **Stats Strided MskMax** project. If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Open a Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For any questions or feedback, feel free to reach out:

- **Email:** your-email@example.com
- **GitHub:** [Korva44](https://github.com/Korva44)

To download the latest version of the library, visit our [Releases section](https://github.com/Korva44/stats-strided-mskmax/releases).

Thank you for checking out **Stats Strided MskMax**! We hope this library helps you with your statistical computations.