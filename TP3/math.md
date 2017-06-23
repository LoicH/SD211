## Préparation 1)

$z = \begin{bmatrix}x \\ Tx \end{bmatrix}$

$A = \begin{bmatrix} I_p \\ T \end{bmatrix}$

## Préparation 2)

$\mathcal L_\rho(x, z, \gamma) = f(x) + g(z) + \gamma^T (Ax - z) + \rho/2 ||Ax - z||_2 \\
 = 1/2 ||y - Hx||_2^2 
 + \iota_{[0,1]^P}(z_1) + \beta ||z_2||_1 
 + <\gamma_1, x-z_1> + <\gamma_2, Tx-z_2>
 + \frac \rho 2 ||\begin{bmatrix} x-z_1 \\ Tx-z_2 \end{bmatrix}||_2$
 
 ## Préparation 3)
 
 $\nabla_x f(x) = H^THx - H^Ty$
 
 $\nabla_x <\gamma, Ax-z> = A^T \gamma$
 
 $\nabla_x \frac \rho 2 ||Ax - z||_2^2 = \rho (A^TAx - A^Tz)$
 
 Donc $\nabla_x \mathcal L_\rho(x, z, \gamma) = (H^TH + \rho A^TA)x -H^Ty + A^T(\gamma - \rho z) $ 
 
 Et $\nabla_{x^{k+1}} = 0 \Leftrightarrow x^{k+1} = (A^T(\rho z - \gamma) + H^T y)(H^T H + \rho A^T A)^{-1}$
 
 ($H^T H + \rho A^T A$ est symétrique positive, donc inversible)