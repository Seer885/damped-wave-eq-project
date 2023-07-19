# damped-wave-eq-project
**Week 1**

Setup Github account and repositories

- Learn about Git & Github

Learn python concepts

- Creating and multiplying matrices via numpy

- Running specific for loops

- Matlab plotting

- Finding derivatives via approximation using the D1 matrix



**Week 2**

Finding second derivatives via approximation using the D2 matrix

- Note how D2 = D1 * D1

- Eigenvalues for D2 are all between -4 and 0

Laid foundations for solving differential equations by noting the following facts

- y'(x) = D1 * y(x)

- y''(x) = D2 * y(x)

- (etc)



**Week 3**

Solving dy/dx = k

- y(x) = h * D1^{-1} * k * [y(0) ; 1 ; 1 ; etc]

Solving dy/dx = f(x)

- y(x) = D1^{-1} * [h*f(x_0)+y(0) ; h*f(x_1) ; h*f(x_2) ; etc]

Solving d2y/dx2 = f(x)

- y'(x) = D1^{-1} * [h*f(x_0)+y'(0) ; h*f(x_1) ; h*f(x_2) ; etc]

- y(x) = D1^{-1} * [h*y'(x_0)+y(0) ; h*y'(x_1) ; h*y'(x_2) ; etc]



**Week 4**

Solving d2y/dx2 = f(x) without going one derivative at a time

Solving dy/dx = k * y

Created an eigenvalues plot for D2



**Week 5**

Solved d2y/dx2=k*y

Figured out 3D graphing in python

Started working on approximating xu{x}=tu{x} with u(x,0)=1.


**Week 6**

Learned more about approximating xu{x}=tu{t} with finite difference method

Started working on approximating xu{x}=tu{t} with professor's special method


