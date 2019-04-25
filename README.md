# MiniAODBphysics2018

## Intructions to run the examples.
```
source /cvmfs/cms.cern.ch/cmsset_default.sh
export SCRAM_ARCH=slc6_amd64_gcc700
cmsrel CMSSW_10_2_9
cd CMSSW_10_2_9/src/
cmsenv
voms-proxy-init -voms cms -valid 192:00
git clone https://github.com/jmejiagu/MiniAODBphysics2018.git myAnalyzers/JPsiKsPAT
cd myAnalyzers/JPsiKsPAT/
git checkout cmssw1029
cd ../..
scram b
cd myAnalyzers/JPsiKsPAT/test/
cmsRun PsikaonRootupler.py
```



