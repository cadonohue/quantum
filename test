from dwave.system.samplers import DWaveSampler
from dwave.system.composites import EmbeddingComposite
# Set Q for the problem QUBO
linear = {('x0', 'x0'): -1, ('x1', 'x1'): -1, ('x2', 'x2'): -1}
quadratic = {('x0', 'x1'): 2, ('x0', 'x2'): 2, ('x1', 'x2'): 2}
Q = dict(linear)
Q.update(quadratic)
# Minor-embed and sample 1000 times on a default D-Wave system
response = EmbeddingComposite(DWaveSampler()).sample_qubo(Q, num_reads=1000)
print(response)

#   x0 x1 x2 energy num_oc. chain_.
# 0  1  0  0   -1.0     288     0.0
# 1  0  0  1   -1.0     393     0.0
# 2  0  1  0   -1.0     319     0.0
# ['BINARY', 3 rows, 1000 samples, 3 variables]
