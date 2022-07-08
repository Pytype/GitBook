# No Divergence loss in Dynamic CPMM

### The instantaneous price

$$
p_X (t) = \frac{k}{w(t)} \cdot \frac{1}{(x-a(t))^2}
$$

$$
p_n(x_n, y_n) = \frac{k}{w} \cdot \frac{1}{(x_n-a)^2}
$$

$$
(x_n-a)^2=\frac{k}{p_nw}
$$



### (x, y)

$$
x_n=\sqrt{\frac{k}{p_nw}} + a
$$

$$
y_n = \frac{\frac{k}{w}}{x_n-a}=\frac{\frac{k}{w}}{\sqrt{\frac{k}{p_nw}} }=\sqrt{\frac{kp_n}{w}}
$$

$$
x_0 = \sqrt{\frac{k}{p_0w}}+a,\, \, \, \, \, \, \, \,y_0 = \sqrt{\frac{kp_0}{w}}
$$



### Value of the pool

$$
V_{p_n}(x_n, y_n)=p_nx_n+y_n, \, \, \, \, \, \, \, \, V_{p_n}(x_0, y_0)=p_nx_0+y_0
$$

$$
V_{p_n}(x_n, y_n)=\sqrt{\frac{kp_n}{w}}+p_na+\sqrt{\frac{kp_n}{w}}=2\sqrt{\frac{kp_n}{w}}+p_na
$$

$$
V_{p_n}(x_0, y_0)=p_n\sqrt{\frac{k}{p_0w}}+p_na+\sqrt{\frac{kp_0}{w}}
$$



### Divergence loss

$$
\delta = \frac{V_{p_n}(x_n, y_n)-V_{p_n}(x_0, y_0)}{V_{p_n}(x_0, y_0)}=\frac{2\sqrt{\frac{kp_n}{w}}+p_na - p_n\sqrt{\frac{k}{p_0w}}-p_na-\sqrt{\frac{kp_0}{w}}}{p_n\sqrt{\frac{k}{p_0w}}+p_na+\sqrt{\frac{kp_0}{w}}}
$$

$$
p_0=p_n=p_{mkt}
$$

$$
\therefore \, \, \delta = \frac{2\sqrt{\frac{kp_{mkt}}{w}}+p_{mkt}a - p_{mkt}\sqrt{\frac{k}{p_{mkt}w}}-p_{mkt}a-\sqrt{\frac{kp_{mkt}}{w}}}{p_{mkt}\sqrt{\frac{k}{p_{mkt}w}}+p_{mkt}a+\sqrt{\frac{kp_{mkt}}{w}}}\, \, \,  =\, \, \,  0
$$

​
