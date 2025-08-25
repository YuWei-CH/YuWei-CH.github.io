---
title: "nifty-ls"
excerpt: "A fast Lomb-Scargle periodogram. It's nifty, and uses a NUFFT!.<br/><img src='/images/Flatiron.jpeg'>"
github: https://github.com/flatironinstitute/nifty-ls
collection: portfolio
---

This work extends nifty-ls, a high-performance Lomb–Scargle periodogram implementation, with multiple Fourier terms harmonic fitting with OpenMP-parallelized / GPU-parallelized methods. We leverage a fast and accurate spreading kernel (the "exponential of semicircle") from the Flatiron Institute Nonuniform Fast Fourier Transform(FINUFFT) to replace the extrapolation method of Press and Rybicki when computing trigonometric sums. To efficiently process large batches of short or variably-sized time series, we introduce a heterobatch model that uses "kernel fusion". This approach wraps the entire workflow—preprocessing, FINUFFT execution, and postprocessing—into a single, per-series C++ pipeline via nanobind. By operating entirely in C++, the model avoids Python’s Global Interpreter Lock (GIL) and integrates seamlessly with OpenMP. This tight coupling allows OpenMP's dynamic scheduling to treat each time series as an independent unit of work, effectively balancing the computational load.