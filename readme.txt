NEURON mod files for the Ca-T current from the paper:
Williams SR, Stuart GJ, Action potential backpropagation and 
somato-dendritic distribution of ion channels in thalamocortical neurons.
J Neurosci. 2000 20:1307-17.

Running the kinetics.hoc simulation file will show 
the activation and inactivation steady-states, the time constants, 
and a family of curves generated modeling the protocols 
indicated in the paper.

Parameters for the Boltzmann equation fitting
the activation (m^3) and inactivation (h) steady states
were those reported in the paper (p.1313).

Half activation/inactivation, 
prepulses, and test pulses, were reported in the paper as 
relative to a resting membrane potential, and the model 
uses the Nerst's equation to calculate the Calcium reversal potential. 
Thus, the model's parameter vrest_cat (the resting potential) 
and the initial values of Calcium concentrations (cao and cai)
need to be defined in hoc.

Time constants were not reported in the paper. In the model,
they have been adjusted to give a reasonable approximation of the
voltage-clamp current traces in Figs.8A-B.
 
Under unix systems:
to compile the mod files use the command 
nrnivmodl 
and run the simulation hoc file with the command 
nrngui kinetics.hoc

Under Windows using NEURON 5.1:
to compile the mod files use the "mknrndll" command.
A double click on the simulation file
kinetics.hoc 
will open the simulation window.

Questions on how to use this model should be directed to
michele.migliore@pa.ibf.cnr.it