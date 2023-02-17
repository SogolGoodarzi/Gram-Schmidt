# Gram-Schmidt
### Introduction to Gram Schmidt
In mathematics, particularly linear algebra and numerical analysis, the Gram–Schmidt process is a method for orthonormalizing a set of vectors in an inner product space, most commonly the Euclidean space equipped with the standard inner product. The Gram–Schmidt process takes a finite, linearly independent set of vectors S for k<=n and generates an orthogonal set S' that spans the same k-dimensional subspace of Rn as S. 

![image](https://user-images.githubusercontent.com/125180530/219682044-1bb10323-230f-4649-9f5e-a93c2e65d0ca.png)

![image](https://user-images.githubusercontent.com/125180530/219682131-e959691d-c32f-4cc6-9629-8d979ee8e015.png)

The application of the Gram–Schmidt process to the column vectors of a full column rank matrix yields the QR decomposition (it is decomposed into an orthogonal and a triangular matrix).

### The Gram Schmidt process
![image](https://user-images.githubusercontent.com/125180530/219682622-984a5db7-0b79-41bd-ae48-b305fb1caeba.png)

where <V, U> denotes the inner product of the vectors v and u. This operator projects the vector v orthogonally onto the line spanned by vector u. If u = 0, we define 
![image](https://user-images.githubusercontent.com/125180530/219683169-528d39b3-a8c5-45cb-8e17-fc02b8a3d1d8.png)

the projection map proj0 is the zero map, sending every vector to the zero vector.

The Gram–Schmidt process then works as follows:

![image](https://user-images.githubusercontent.com/125180530/219686395-8fb4967d-bb65-458d-95a9-372074b4ee5e.png)

The sequence u1, ..., uk is the required system of orthogonal vectors, and the normalized vectors e1, ..., ek form an orthonormal set. The calculation of the sequence u1, ..., uk is known as Gram–Schmidt orthogonalization, while the calculation of the sequence e1, ..., ek is known as Gram–Schmidt orthonormalization as the vectors are normalized.

To check that these formulas yield an orthogonal sequence, first compute <u1,u2> by substituting the above formula for u2: we get zero. Then use this to compute <u1,u3> again by substituting the formula for u3: we get zero. The general proof proceeds by mathematical induction.

![image](https://user-images.githubusercontent.com/125180530/219688712-82c1d0cd-50f6-4bd9-9202-bf0e1c44edc7.png)

* In the first step of this project, we implement the Gram Schmidt algorithm.

* Now we improve the algorithm and create the Changed_Gram_Schmidt function for this purpose.

* Finally, we can test these two algorithms using the below example:

![image](https://user-images.githubusercontent.com/125180530/219689997-e5b0e944-f5cc-4dfc-bd58-fd9d870acae5.png)
