# SFrameAnalysis

Code for skimming UZH ntuples for top/W tagging scalefactor calculations

## Getting started

You need ROOT or CMSSW to get started, here CMSSW will be used, and the installation will be done into a new directory:
```
source /cvmfs/cms.cern.ch/cmsset_default.sh
cmsrel CMSSW_8_0_20
cd CMSSW_8_0_20/src
cmsenv
cd ../..
```
Get the right branch and get SFrame:
```
git checkout -b VTopScalefactor origin/VTopScalefactor
source init.sh
```

Setup and compile SFrame:
```
cd SFrame
source setup.sh
make
cd ..
```

## Compilation

To compile all submodules:
```
source make.sh
```
To ```make distclean``` for all submodules:
```
source makedistclean.sh
```
Mind that SFrame itself and any other directory, which is not a submodule, will not be touched.

## Further documentation

Please read https://git-scm.com/book/en/v2/Git-Tools-Submodules for information on how to work with submodules.