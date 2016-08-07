# snake_matlab

matlab codes download from line, this is a very good material 

Build matrix A using circshift
for i=1:m
    A(i,:) = brow;
    brow = circshift(brow',1)'; % Template row being rotated to egenrate different rows in pentadiagonal matrix
end

Also, the inverse of A is computed by LU decomposition

[L U] = lu(A + gamma .* eye(m,m));
Ainv = inv(U) * inv(L); % Computing Ainv using LU factorization
