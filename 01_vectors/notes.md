# Vectors — Linear Algebra

Vectors are one of the most important building blocks of **Linear Algebra**. They are widely used in Mathematics, Computer Science, Machine Learning, Computer Graphics, Physics, Robotics, Computer Vision, and many other fields.

This README provides a simple introduction to vectors and explains why they are important in Computer Science.

---

## 1. What is a Vector?

A vector is a mathematical object that contains a collection of numbers.

For example:

```text
v = [2, 4, 6]
```

This is a vector containing three numbers.

A normal number is called a **scalar**:

```text
5
```

A vector contains multiple values:

```text
[2, 4, 6]
```

So:

```text
Scalar → 5
Vector → [2, 4, 6]
```

---

## 2. What Does a Vector Represent?

A vector can represent different things depending on the problem.

For example:

```text
[10, 20]
```

could represent:

- A point in 2D space
- A direction
- Position `(x, y)`
- Temperature and humidity
- Two features of a dataset

Similarly:

```text
[10, 20, 30]
```

could represent:

- A point in 3D space
- RGB color values
- Three features of a machine-learning dataset

The meaning of a vector depends on the context.

---

## 3. Vectors in Geometry

A 2D point such as:

```text
(3, 4)
```

can be represented as:

```text
v = [3, 4]
```

This vector tells us:

- Move 3 units in the x-direction
- Move 4 units in the y-direction

Vectors can therefore represent both **position** and **direction** in geometry.

---

## 4. Dimension of a Vector

The number of values inside a vector is called its **dimension**.

```text
[5]              → 1 dimension
[2, 4]           → 2 dimensions
[2, 4, 6]        → 3 dimensions
[1, 2, 3, 4, 5]  → 5 dimensions
```

In general:

```text
v = [x₁, x₂, x₃, ..., xₙ]
```

is an **n-dimensional vector**.

---

## 5. Components of a Vector

Each individual value inside a vector is called a **component**.

For:

```text
v = [3, 7, 2]
```

we have:

```text
v₁ = 3
v₂ = 7
v₃ = 2
```

So the vector has three components.

---

## 6. Vector Addition

Two vectors of the same dimension can be added by adding their corresponding components.

```text
a = [2, 3]
b = [4, 5]

a + b = [2 + 4, 3 + 5]
      = [6, 8]
```

Therefore:

```text
[2, 3] + [4, 5] = [6, 8]
```

---

## 7. Scalar Multiplication

A vector can be multiplied by a scalar.

```text
v = [2, 4, 6]

3v = 3[2, 4, 6]
   = [6, 12, 18]
```

The scalar multiplies every component of the vector.

---

## 8. Vector Subtraction

Vectors can also be subtracted component by component.

```text
a = [8, 6]
b = [3, 2]

a - b = [8 - 3, 6 - 2]
      = [5, 4]
```

---

## 9. Magnitude of a Vector

The **magnitude**, or length, of a vector tells us how large the vector is.

For a 2D vector:

```text
v = [x, y]
```

its magnitude is:

```text
|v| = √(x² + y²)
```

Example:

```text
v = [3, 4]

|v| = √(3² + 4²)
    = √25
    = 5
```

For an n-dimensional vector:

```text
v = [x₁, x₂, ..., xₙ]
```

the magnitude is:

```text
|v| = √(x₁² + x₂² + ... + xₙ²)
```

---

## 10. Dot Product

The **dot product** is one of the most important operations involving vectors.

Suppose:

```text
a = [2, 3]
b = [4, 5]
```

Then:

```text
a · b = (2 × 4) + (3 × 5)
      = 8 + 15
      = 23
```

So:

```text
a · b = 23
```

The dot product produces a **scalar**, not another vector.

---

## 11. Why is the Dot Product Important?

The dot product tells us about the relationship between two vectors.

It is related to the angle between them:

```text
a · b = |a||b|cos(θ)
```

Because of this, dot products are useful for determining how similar the directions of two vectors are.

This becomes very important in:

- Machine Learning
- Neural Networks
- Computer Vision
- Natural Language Processing
- Information Retrieval
- Recommendation Systems

---

# 12. Vectors in Computer Science

Vectors are extremely important in Computer Science because many types of information can be represented using numbers.

Once information is converted into numbers, it can often be represented as a vector.

For example, a student might have:

```text
Math Score      = 85
Programming     = 90
Physics         = 75
```

We can represent the student as:

```text
student = [85, 90, 75]
```

This vector represents the student's characteristics.

This idea is fundamental to **Machine Learning**.

---

# 13. Vectors in Machine Learning

Machine Learning models work with numerical data.

Suppose we want to predict the price of a house.

We might have:

```text
Size       = 1200 sq ft
Bedrooms   = 3
Age        = 10 years
```

We can represent this information as:

```text
house = [1200, 3, 10]
```

Each value is called a **feature**.

Therefore:

```text
Vector = [feature₁, feature₂, feature₃, ...]
```

A dataset can be viewed as many vectors:

```text
House 1 → [1200, 3, 10]
House 2 → [1500, 4, 5]
House 3 → [900, 2, 20]
```

The ML model learns patterns from these numerical representations.

---

# 14. Vectors in Neural Networks

Neural networks heavily depend on vector operations.

A simple neuron performs an operation similar to:

```text
output = w · x + b
```

where:

```text
x = input vector
w = weight vector
b = bias
```

For example:

```text
x = [2, 3]
w = [0.5, 0.8]
```

The neuron calculates:

```text
w · x
= (0.5 × 2) + (0.8 × 3)
= 1 + 2.4
= 3.4
```

Then the bias is added.

This type of vector operation is repeated many times inside neural networks.

---

# 15. Vectors in Deep Learning

Deep-learning systems process huge amounts of numerical data.

For example, a grayscale image can be represented as a matrix of pixel values:

```text
[0,   50,  120]
[200, 255, 80 ]
[10,  100, 180]
```

These values can eventually be represented as vectors or higher-dimensional arrays called **tensors**.

Similarly:

- Text → numerical vectors
- Images → numerical arrays
- Audio → numerical arrays
- Video → numerical arrays

This allows neural networks to process different types of information.

---

# 16. Vectors and Embeddings

One of the most important modern applications of vectors is **embeddings**.

An embedding converts something such as a word, sentence, image, or document into a vector.

For example:

```text
"king" → [0.21, -0.45, 0.73, ...]
```

```text
"queen" → [0.19, -0.42, 0.70, ...]
```

These vectors can contain hundreds or thousands of dimensions.

The important idea is that objects with similar meanings can have similar vector representations.

For example:

```text
"cat"    → vector A
"kitten" → vector B
"car"    → vector C
```

Vector A and B may be closer to each other than A and C.

Embeddings are widely used in:

- Large Language Models
- Search engines
- Recommendation systems
- Semantic search
- Natural Language Processing
- Computer Vision

---

# 17. Vectors in Computer Graphics

Vectors are heavily used in computer graphics.

A position can be represented using a vector.

2D:

```text
Position = [x, y]
```

3D:

```text
Position = [x, y, z]
```

Vectors can represent:

- Position
- Direction
- Velocity
- Acceleration
- Surface normals
- Camera orientation

For example:

```text
Player position = [10, 5, 2]
```

A game engine can use this vector to determine where the player exists in a 3D world.

---

# 18. Vectors in Robotics

Robots operate in physical space, so vectors are extremely useful.

A robot's position might be:

```text
P = [x, y, z]
```

Its velocity might be:

```text
V = [vx, vy, vz]
```

Vectors can therefore describe:

- Position
- Movement
- Velocity
- Force
- Rotation
- Sensor data
- Robot control

---

# 19. Vectors in Computer Vision

Computer vision deals with images and videos.

An RGB pixel can be represented as:

```text
[255, 0, 0]
```

which represents a red color.

A larger image contains millions of numerical values.

Machine-learning models can transform image information into high-dimensional numerical representations.

These representations are often treated as vectors.

---

# 20. Vectors in Natural Language Processing

Computers cannot directly process words in the same way humans understand them.

Words can be converted into numerical vectors.

For example:

```text
"apple" → [0.12, 0.45, -0.21, ...]
```

```text
"orange" → [0.10, 0.41, -0.19, ...]
```

These vector representations allow mathematical operations to be performed on language.

Modern NLP systems use high-dimensional vector representations extensively.

---

# 21. Vectors in Search Engines

Suppose you search:

```text
"best laptop for programming"
```

A search system can convert the query into a vector.

Documents can also be converted into vectors.

The system can then compare the query vector with document vectors.

Conceptually:

```text
Query
  ↓
Vector
  ↓
Compare with document vectors
  ↓
Find similar vectors
  ↓
Return relevant results
```

This is the basic idea behind **semantic search**.

---

# 22. Vectors in Recommendation Systems

Recommendation systems can also use vectors.

For example, a user can be represented using a vector:

```text
User = [0.8, 0.2, 0.9, 0.1]
```

A movie can also be represented using a vector:

```text
Movie = [0.7, 0.3, 0.8, 0.2]
```

If the vectors are similar, the system may consider the movie a good recommendation for the user.

This basic idea is used in:

- Movie recommendations
- Music recommendations
- Product recommendations
- Content recommendations

---

# 23. Vectors Are Everywhere

The important idea to remember is:

> **If information can be represented using numbers, it can often be represented using vectors.**

Examples:

```text
Student
   ↓
[85, 90, 75]

Image
   ↓
[120, 34, 255, ...]

Word
   ↓
[0.21, -0.43, 0.72, ...]

Robot position
   ↓
[10, 5, 2]

House
   ↓
[1200, 3, 10]
```

Different fields use vectors for different purposes.

---

# 24. Important Vector Concepts to Learn Next

After understanding the basics, the next concepts to study are:

1. Vector addition
2. Vector subtraction
3. Scalar multiplication
4. Magnitude / Norm
5. Unit vectors
6. Dot product
7. Cross product
8. Angle between vectors
9. Orthogonality
10. Projection
11. Linear combinations
12. Linear independence
13. Basis
14. Span
15. Vector spaces
16. Matrices
17. Eigenvalues and eigenvectors

These concepts form the foundation for understanding more advanced topics in Linear Algebra.

---

# 25. Why Vectors Matter for Machine Learning

A large part of Machine Learning can be understood as performing mathematical operations on vectors and matrices.

A simplified view is:

```text
Data
 ↓
Vectors
 ↓
Matrices
 ↓
Mathematical operations
 ↓
Model
 ↓
Prediction
```

Later, concepts such as:

- Gradient Descent
- Neural Networks
- Backpropagation
- Principal Component Analysis
- Linear Regression
- Transformers
- Embeddings

all make extensive use of vectors and matrices.

Therefore, having a strong understanding of vectors makes many Machine Learning concepts easier to understand.

---

# Quick Summary

### Vector

A collection of numbers:

```text
v = [2, 4, 6]
```

### Dimension

Number of components:

```text
[2, 4, 6] → 3 dimensions
```

### Addition

```text
[1, 2] + [3, 4]
= [4, 6]
```

### Scalar Multiplication

```text
3[1, 2]
= [3, 6]
```

### Magnitude

```text
|v| = √(x₁² + x₂² + ... + xₙ²)
```

### Dot Product

```text
a · b = Σ(aᵢbᵢ)
```

### Main Idea

```text
Real-world information
        ↓
Numbers
        ↓
Vectors
        ↓
Mathematical operations
        ↓
Computer Science applications
```

Vectors are therefore not just a mathematical concept. They are one of the fundamental ways computers represent and process information.
