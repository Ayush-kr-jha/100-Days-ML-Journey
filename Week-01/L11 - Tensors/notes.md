# Tensors :

1. Scalar : a single numerical value, represented as a 0-dimensional tensor. Example: 5, -3.2 , a = np.array(7)
2. Vector : an ordered array of numbers, represented as a 1-dimensional tensor. Example: [2, 4, 6] or v = np.array([1, 3, 5])
3. Matrix : a 2-dimensional array of numbers, represented as a 2-dimensional tensor 
    - Example: 
        np.array([[1, 2, 3],
                  [4, 5, 6],
                  [7, 8, 9]])
      ```
      [[1, 2, 3],
        [4, 5, 6],
        [7, 8, 9]]
      ```
4. Higher-Dimensional Tensors : tensors with three or more dimensions, used to represent more complex data structures.
    - Example: A 3-dimensional tensor representing a color image with height, width, and color channels (RGB).

    np.array([[[255, 0, 0], [0, 255, 0], [0, 0, 255]],
              [[255, 255, 0], [0, 255, 255], [255, 0, 255]]])

      ```
      [[[255, 0, 0], [0, 255, 0], [0, 0, 255]],
       [[255, 255, 0], [0, 255, 255], [255, 0, 255]]]
      ```   
    - Example: A 4-dimensional tensor representing a batch of images, with dimensions for batch size, height, width, and color channels.
    np.array([[[[255, 0, 0], [0, 255, 0]], 
                 [[0, 0, 255], [255, 255, 0]]],
                
                [[[0, 255, 255], [255, 0, 255]], 
                 [[192, 192, 192], [128, 128, 128]]]])
      ```
      [[[[255, 0, 0], [0, 255, 0]], 
        [[0, 0, 255], [255, 255, 0]]],
       
       [[[0, 255, 255], [255, 0, 255]], 
        [[192, 192, 192], [128, 128, 128]]]]
      ```

# Rank, Shape, and Size of Tensors :
1. Rank : the number of dimensions a tensor has. (no. of axis = rank = no. of dimensions)
    np.array(5)            # Rank 0
    np.array([1, 2, 3])    # Rank 1 - 1D Tensor but Vector dimension is (3,)
    np.array([[1, 2], [3, 4]])  # Rank 2 - 2D Tensor but Matrix dimension is (2,2)
    np.array([[[1], [2]], [[3], [4]]])  # Rank 3 - 3D Tensor but dimension is (2,2,1)
    np.array([[[[1]], [[2]]], [[[3]], [[4]]]])  # Rank 4 - 4D Tensor but dimension is (2,2,1,1)

    ndim attribute can be used to get the rank of a tensor.
    - arr.ndim   #returns the rank of the tensor

    - Scalar : Rank 0
    - Vector : Rank 1
    - Matrix : Rank 2
    - Higher-Dimensional Tensors : Rank 3 or more



2. Shape : the size of each dimension of the tensor, represented as a tuple.
    - Example: A matrix with 3 rows and 4 columns has a shape of (3, 4).
    - Example: A 3-dimensional tensor with dimensions 2x3x4 has a shape of (2, 3, 4).
    - The shape attribute can be used to get the shape of a tensor.
    - arr.shape   # returns the shape of the tensor



3. Size : the total number of elements in the tensor, calculated by multiplying the sizes of all dimensions.
    - Example: A matrix with shape (3, 4) has a size of 12 (3 * 4 = 12).
    - Example: A 3-dimensional tensor with shape (2, 3, 4) has a size of 24 (2 * 3 * 4 = 24).
    - The size attribute can be used to get the size of a tensor.
    - arr.size   # returns the total number of elements in the tensor



# Summary Table :
| Tensor Type               | Rank | Shape Example     | Size Example |
|---------------------------|------|-------------------|--------------|
| Scalar                    | 0    | ()                | 1            |
| Vector                    | 1    | (3,)              | 3            |
| Matrix                    | 2    | (3, 4)            | 12           |
| Higher-Dimensional Tensor | 3+   | (2, 3, 4)         | 24           |
