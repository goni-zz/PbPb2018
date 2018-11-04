# PbPb2018
## for MkBatch
```bash
cmsrel CMSSW_10_3_1
git clone 
cp HiSkim/HiOnia2MuMu/python/onia2MuMuPAT_cff.py
vi HiSkim/HiOnia2MuMu/python/onia2MuMuPAT_cff.py
52         process.muonL1Info.matched = cms.InputTag("gtStage2Digis:Muon:RECO") #get correctly L1
```
t0 streamer
```bash
python submitForestStreamer.py -q 1nd -o /eos/cms/store/group/phys_heavyions/dileptons/Data2018/PbPb502TeV/TTrees/test/ -i 325112.txt
```
prompt reco
```bash
python submitForestPR.py 'same with above'
```
express stream
```bash
python submitForestExpress.py 'same with above'
```
