# spike2vec
Pre-print doc at first fading into full code repository.

[Spike2vec manuscript draft](main.pdf)



=== Virtual Experiment Simulation Protocol

We presented neuromorphic data to the potjan's network model. To do this we constructed
a 2D population layer, and gave every cell spatial coordinates. We systematically populated cell centres along a 2D grid. 
/*randomly populated a 2D sheet with x,y coordinates so that we could give each cell a unique spatial position.
We then applied a distance dependent wiring rule to the input layer, */

We then used a distance dependent wiring rule such that neighbouring cells are more likely to be synaptically connected with each other with inhibitory synapses, according to a "winner-take-all" connection scheme.
This 2D sheet population of cells then mapped onto regular 1D populations of cells, in the Potjan's balanced E/I model.

In this way we were able to present several neuromorphic data types to the Potjan's E/I network, 
and we allowed the network to train its synapses with STDP synaptic update rules. 
under exposure to 5 out of 10 different numbers of the NMNIST neuromorphic data set.

We used the spike2vec algorithm from @cite_self_preb to show that presenting familiar training items (0-2-4-6-8) to the trained model caused the network to enter attractors (caused the network to recall a repeated temporal spatial pattern).
Presenting un-familiar NMNIST items (odd numbers 1-3-5-7-9), did not cause the network to enter those attractors as frequently.

We also applied the Recurrence Analysis metrics to its found state transition matrices, for spike2vec encoded raster plot evolutions under both familiar and unfamiliar item categories.
Finally we converted the spike sequence vectors to word vectors, on trained familiar items, and trained unfamiliar items. Converting spikes to words via vectors, allowed us to compare model spike trains with emperical data, using the statistics of natural language.
