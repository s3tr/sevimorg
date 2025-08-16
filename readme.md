# **FPACK/FUNPACK Precision Loss Calculator**

This web-based tool simulates and analyzes the precision loss from converting a 32-bit floating-point number to a custom 16-bit format and back, mimicking the FPACK and FUNPACK instructions of the ADSP-214xx SHARC processor. The loss is caused by the reduction in bits used for the mantissa and exponent during the conversion process.

## **How It Works**

The application's core JavaScript functions simulate the FPACK (32-bit to 16-bit) and FUNPACK (16-bit to 32-bit) conversion. FPACK truncates the mantissa and clamps the exponent, causing rounding and quantization errors. The **precision loss** is the absolute difference between the original and final 32-bit floating-point values.

## **Features**

* **Generate Single Number:** Test a single random number to see its converted value, loss, and 16-bit binary representation.  
* **Generate Batch:** Test 1000 random numbers to calculate the average precision loss.  
* **Interactive UI:** A modern, browser-based interface for easy visualization of results.

## **Technologies Used**

* **HTML:** For the document structure.  
* **Tailwind CSS:** For all styling and responsive design.  
* **JavaScript:** For the core logic and UI interaction.

## **Getting Started**

To use the application, simply open the index.html file in any modern web browser.

1. Click **"Generate Single Number"** to test a single value.  
2. Click **"Generate Batch (1000)"** to run a large-scale test.