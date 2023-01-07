---
title: Setup
---
# Computing Environment at FNAL LPC


The code snippets below describe the steps to follow to login at the LPC cluster and set up the necessary working area for this twiki. The requirements described in **Prerequisites** are necessary to proceed to this step.

Login on LPC cluster:

```shell
kinit yourlpcusername@FNAL.GOV
ssh -Y yourlpcusername@cmslpc-sl7.fnal.gov
```


Create a working directory in your nobackup area:

```shell
cd ~/nobackup
mkdir TauTauLongExercise
cd TauTauLongExercise
```

Setup CMSSW framework:
```shell
# bash?
source /cvmfs/cms.cern.ch/cmsset_default.sh
# or tcsh?
source /cvmfs/cms.cern.ch/cmsset_default.csh

set SCRAM_ARCH=slc7_amd64_gcc700
cmsrel CMSSW_10_6_27
cd CMSSW_10_6_27/src
cmsenv
```

Pull in the repository with analysis and ntuple code:

```shell
git clone --single-branch --branch cmsdas2022 https://github.com/fojensen/nanoAOD-tools.git PhysicsTools/NanoAODTools
scram build
```

Connect to the grid:

```shell
voms-proxy-init -voms cms
```
<p style="height: 100px"></p>


{% include links.md %}
