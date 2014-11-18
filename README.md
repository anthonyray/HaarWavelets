# Haar Wavelet Transformation

This is a simple implementation of one dimensional and two dimensional Haar Wavelets Transformation.

For each transformation, the input is a 1D or 2D array of double, and the output is a 1D or 2D array of double.

## Usage

### One dimensional Haar Wavelet transformation
Let's take the following example. We have a 1D array of double.

```java
double[] data = {9, 7, 3, 5 };
```
We instantiate a class to transform the matrix :

```java
HaarWavelet1D oneD = new HaarWavelet1D(data);
oneD.standardDecomposition();
```

The result is :
```
Processing One Dimensional Haar Wavelet Transformation
Input :
9.0, 7.0, 3.0, 5.0
Output :
6.0, 2.0, 1.0, -1.0
```

### Two dimensional Haar Wavelet transformation

Let's take the following example : We have a 2D array of double.

```java
double[][] data2D = {{9, 7, 3, 5 },{2, 4, 8, 4 },{1, 7, 13, 4 },{19, 27, 53, 45 }};

HaarWavelet2D twoD = new HaarWavelet2D(data2D);

```

The result is the following :
```
Processing Two Dimensional Haar Wavelet Transformation
Input :
9.0, 7.0, 3.0, 5.0
2.0, 4.0, 8.0, 4.0
1.0, 7.0, 13.0, 4.0
19.0, 27.0, 53.0, 45.0

Output :
13.1875, -3.6875, -1.75, 2.375
-7.9375, 3.9375, 1.75, -1.875
0.75, 1.75, 1.0, -1.5
-14.875, 5.375, 0.5, 0.25
```
