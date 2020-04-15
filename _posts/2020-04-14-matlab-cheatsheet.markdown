---

layout: post

title:  "Householder transformation"

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
