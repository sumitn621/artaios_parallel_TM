# artaios_parallel_TM
## For running program ```artaios``` in parallel for Turbomole output
Running transport calculations in parallel there is a nice tool from Ryan Chiechis's group named ```QuantumParse``` which can be found at https://github.com/rchiechi/QuantumParse. The sub-tool ```ArtaiosParallel.py``` can be used to distribute the transmission calculations in separate processors depending on the energy ranges. After finishing the calculations all the values of transmission at different energies are stored in the transmission.1.dat file where no order is maintained ( ```use: sort -nk 1 transmission.1.dat > transmission_ordered.dat```). The program is super nice and can be used for ```Gaussian``` and ```orca 4```. I have edited the ```ArtaiosParallel.py``` program a bit so that it can be used for ```Turbomole V>=7``` output as well. The modified program named ```ArtaiosParallel_TM.py``` with test input file for ```artaios``` named ```transport.in``` can be found in this repository.
