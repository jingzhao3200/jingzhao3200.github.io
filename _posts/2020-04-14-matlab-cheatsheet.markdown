---

layout: post

title:  "Matlab Cheatsheet"

date: 2020-04-14 00:03:49 -0400

categories: jekyll update

---

### cat
#### Syntax
C = cat(dim,A,B)
C = cat(dim,A1,A2,…,An)

#### Description
C = cat(dim,A,B) concatenates B to the end of A along dimension dim when A and B have compatible sizes (the lengths of the dimensions match except for the operating dimension dim).

#### example

A = ones(3)
A = 3×3

     1     1     1
     1     1     1
     1     1     1

B = zeros(3)
B = 3×3

     0     0     0
     0     0     0
     0     0     0

C1 = cat(1,A,B)
C1 = 6×3

     1     1     1
     1     1     1
     1     1     1
     0     0     0
     0     0     0
     0     0     0

C2 = cat(2,A,B)
C2 = 3×6

     1     1     1     0     0     0
     1     1     1     0     0     0
     1     1     1     0     0     0
     
### repmat
Repeat copies of arraycollapse all in page
#### Syntax
B = repmat(A,n)
B = repmat(A,r1,...,rN)
B = repmat(A,r)
#### Description
#### example
B = repmat(A,n) returns an array containing n copies of A in the row and column dimensions. The size of B is size(A)*n when A is a matrix.

#### example
B = repmat(A,r1,...,rN) specifies a list of scalars, r1,..,rN, that describes how copies of A are arranged in each dimension. When A has N dimensions, the size of B is size(A).*[r1...rN]. For example, repmat([1 2; 3 4],2,3) returns a 4-by-6 matrix.

#### example
B = repmat(A,r) specifies the repetition scheme with row vector r. For example, repmat(A,[2 3]) returns the same result as repmat(A,2,3).

#### Examples

Create a 3-by-2 matrix whose elements contain the value 10.

A = repmat(10,3,2)
A = 3×2

    10    10
    10    10
    10    10

