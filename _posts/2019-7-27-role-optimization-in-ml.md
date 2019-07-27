---
layout: post
title: The role of Optimization in Statistics and Machine Learning
---

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

My current professional work involves, in general terms, is what I would call computational Statistics. This requires using current statistical packages, but also experimenting with open source software. It often includes tweaking the algorithms to suit to big data requirements. Since most machine learning or statistical modeling uses empirical risk minimization or maximum likelihood estimation, the underlying algorithms behind the models uses optimization.

$$\min E[\text{max}\{0, a_1x_1+\cdots+a_nx_n -b\}]\approx
                        \left\{ \begin{array}{ll}
                         \min \sum_{k=1}^{K}{\pi_kv_k}&\\
                        \text{s.t.}&\\
                        v_k\geq 0&\forall k\\
                        v_k\geq a_1x_1+\cdots+a_nx_n -b_k&\forall k\\
                        \end{array}
                        \right.$$





