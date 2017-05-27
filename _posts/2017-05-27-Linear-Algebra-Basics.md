---
layout: post
title: "anilmullapudi, Launches Site"
date: 2017-05-27
---

<p>
<b>Vector : </b>  A vector is line in Cartesian space with a direction.  example: a=[2;3]
vector can be 1-dimensional, 2-dimensional, 3-dimensional....upto n-dimensional.
</p>


<p>
<b>Linear Transformations:</b> If a vector is multiplied with a matrix, it may change its direction and spanning in its size.  example: a vector a=[2 3]  is multiplied by a matrix T= [3 1; 2 2] ,  a new vector is formed with dimension [12, 8].     This new vector has different length and direction when compared to original vector 'a [2]'. Again, transformation can be applied on more than one dimensional vectors.
</p>



<p>
<b>Determinant:</b>  If a matrix with a dimension 2x2, that means it contains two vector.  Each column represents one vector.  If we plot and extend these two vectors in a Cartesian space, we can compute the area(A) under these vectors.  Determinant is a factor value that describes how much the  area 'A' from a unit vectors. Overall, the determinant is a way to compute the are covered by vectors present in the matrix.

ex:  matrix x = [3 2; 1 2] , its determinant |x| = ad-bc =  4.   Therefore the area is 4.

If the determinant of a matrix is zero, then there is no area under those vectors. that means all the vectors are on the same line or direction.  We can call these vectors linearly dependent.  because we can determine one vector from another vector by scaling.
</p>



<p>
<b>Rank:</b>
Any matrix after a linear transformation, it may change in its dimensions. A rank represents these dimensions. Suppose, a 3 dimensional vector is converted into 2 dimensional after transformation. Then its rank is 2.  if, after the transformation output vector is a three dimension then that matrix has the rank 3.
</p>



<p>
<b>Inverse of a matrix:</b>   If we transformed a matrix 'A' by using a transformation matrices.  After transformation the original matrix is transformed and rotated. If we want the original matrix from the transformed matrix, then we need to multiply with inverse matrix.  Therefore, inverse matrix undo all the changes and gives original matrix. 
</p>



<p>
<b>Singular Matrix :</b> A square matrix that is not in-veritable is called singular matrix. 
   
According to singular matrix definition, matrix A do not have inverse. That is in the above formula the determinant is zero.
</p>



<p>
<b>Diagonal Matrix:</b>  Any matrix whose diagonals has some values and remaining all the values are zero's then its a diagonal matrix. These diagonals are also called eigen values.
</p>



<p>
<b>Eigen vectors:</b>  Suppose a matrix 'A' contains many vectors in it, and we performed transformations on 'A'.  If the transformed matrix contains any vectors that are not change in its direction, that is parallel to original vectors, then these vectors are called eigen vectors.   In other words,   the vectors remains constant after transformation are eigen vectors.  But eigen vectors can be scaled to in the same direction after the transformation. This scaling factors are called eigen values.  
</p>



<p>
<b>Basis vectors:</b> Mostly we plot the vectors from the origin (0,0).  But its not mandatory, others may plot the same point from different region.  Therefore, depending on the basis vectors the representation of the point will change and we need to use transformations and rotations to convert a point from one basis to another basis vectors.   Choosing a eigen vectors as a basis is a good implementation, because the matrix operations on eigen vectors are much simpler. If we are able to convert the normal vectors into eigen basis the basis is called 'Eigenbasis'.  For instance, we have a transformation matrix and we want to calculate the 100th power it.  If we can convert this transformation into to 'Eigenbasis', we get a diagonal matrix. We can easily we perform 100th power on this and transform back to original basis.  
</p>



<p>
<b>SVD (Singular value decomposition) :</p>  SVD is a function that generates the Eigen vectors, Eigen Values(diagonal matrix) and other rotation matrix.

If a vector 'v' is multiplied with matrix 'M', then a new vector 'u' will be formed.   However, the new vector 'u' will rotate and translate from the original vector 'v'. This entire process can be shown in the following equation.
                                                       v * M = u, alpha
Here, v is vector in some directional (rotational matrix), u is new vector (rotational matrix)
alpha is the amount of translation in 'u'. (translation matrix)

Now, apply the above concept into multi-dimensional space, that is our input 'v' can have many vectors, and then the output 'u' also will have corresponding new vectors and translations. This can be represented as    
                        V * M = U * S  ----> equation1
Here S is sigma, it's a transnational matrix which is also called as diagonal matrix.  Because, S tells us how much 'U' will be extended or translated in 'U' vector space.   Now, multiply both sides of equation-1 with a inverse of V, then we get the below equation. 
                       M = U * S * ~V   this is a singular value decomposition.
here ~V represents inverse of V,  U is a eigen vectors (each vector is orthogonal), S is a diagonal matirx also called as eigen value matrix, ~V is a rotational matrix.

Note: now take any vector and multiply with U from the above equation.  The resultant matrix is nothing but a projection from the Eignebasis.

</p>
