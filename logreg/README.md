To Use!

untar data.tar.bz2
run RUNCHPLDEMO.sh and RUNPYDEMO.sh

Notes!

The Python implementation performs a shuffle
over the training samples prior to running
the training algorithm.

The Chapel implementation does not currently
perform a shuffle over training samples prior
to running the training algorithm.

The training sample shuffle is not included 
in timing the algorithm.

Since the algorithm does not perform iterations
optimizing an objective function (it's a 
stochastic algorithm) but instead trains over
all available examples, holding out 'shuffle'
should have no impact the algorithm's 
runtime/execution performance. The lack of a
shuffle will impact statistical performance.
