%% Lab1 - Ignas Laude MAT343
% MAT 343 MATLAB Assignment # 1

%% Question # 1
A = [1, 2; 3, 6]

B = [2, -3; 1, 4]

C = [-2, 1; 3, 2]

%% Question #2

%(a)

A + B

B + A

% They are the same

%%

%(b)

(A+B)+C

A+(B+C)

% Matrix Addition follows the associative property so they are the same


%%

%(c)

x = 6

x*(A+B)

x*A + x*B

% Yes, they are the same

%% 

%(d)

A*(B+C)

A*B + A*C

% Multiplication is distributive in this case so it is the same

%%
% (e)

% (i)
A*B

A*C
%%
% (ii)
A*B

B*A

%%

% (f)

% (i)
A * B

[A*B(:,1), A*B(:,2)]

% (ii)
A*B

[A(1,:)*B; A(2,:)*B]

% (iii)
% Matrix (i) is computed by first calling the first column of matrix B and multiplying it by Matrix A
   % then for the bottom row we call the second column of matrix B and multiply it by matrix A
   
% Matrix (ii) is computed by calling the first row of Matrix A and then multiplying it by matrix B
   % then for the bottom row the second row of matrix A is then multiplied by matrix B
   
%% Question 3 

M = [eye(3) * 2]

N = [zeros(2,2)]

P = ones(3,3)*3, triu(P,0)

Q = [ones(2,3) * 4]

%% Question 4

G = [A, eye(2, 2), N; N, B, eye(2, 2); eye(2, 2), N, C]

%% Question 5

%(a)

H = G(1:3, 1:3)

%(b)

E = H

E(3:3, 3:3) = 5

E

%(c)

H(2, :) = []

F = H

F

%(d)

% G(:,:) - Since it called all the columns and all the rows nothing visibly
% changed

% G(:) - Every value is return and placed into a single column vector
% (36x1) Matrix

%(e)

 G(8)
 
% The value 6 was returned which was the 8th iteratio%% Lab1 - Nikola Uzelac MAT343
% MAT 343 MATLAB Assignment # 1

%% Question # 1
A = [1, 2; 3, 6]

B = [2, -3; 1, 4]

C = [-2, 1; 3, 2]

%% Question #2

%(a)

A + B

B + A

% They are the same

%%

%(b)

(A+B)+C

A+(B+C)

% Matrix Addition follows the associative property so they are the same


%%

%(c)

x = 6

x*(A+B)

x*A + x*B

% Yes, they are the same

%% 

%(d)

A*(B+C)

A*B + A*C

% Multiplication is distributive in this case so it is the same

%%
% (e)

% (i)
A*B

A*C
%%
% (ii)
A*B

B*A

%%

% (f)

% (i)
A * B

[A*B(:,1), A*B(:,2)]

% (ii)
A*B

[A(1,:)*B; A(2,:)*B]

% (iii)
% Matrix (i) is computed by first calling the first column of matrix B and multiplying it by Matrix A
   % then for the bottom row we call the second column of matrix B and multiply it by matrix A
   
% Matrix (ii) is computed by calling the first row of Matrix A and then multiplying it by matrix B
   % then for the bottom row the second row of matrix A is then multiplied by matrix B
   
%% Question 3 

M = [eye(3) * 2]

N = [zeros(2,2)]

P = ones(3,3)*3, triu(P,0)

Q = [ones(2,3) * 4]

%% Question 4

G = [A, eye(2, 2), N; N, B, eye(2, 2); eye(2, 2), N, C]

%% Question 5

%(a)

H = G(1:3, 1:3)

%(b)

E = H

E(3:3, 3:3) = 5

E

%(c)

H(2, :) = []

F = H

F

%(d)

% G(:,:) - Since it called all the columns and all the rows nothing visibly
% changed

% G(:) - Every value is return and placed into a single column vector
% (36x1) Matrix

%(e)

 G(8)
 
% The value 6 was returned which was the 8th iteratio
