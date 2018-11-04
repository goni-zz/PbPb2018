# PbPb2018
## CMSSW_10_3_1
HiSkim/HiOnia2MuMu/python/onia2MuMuPAT_cff.py
puth line
```bash
52         process.muonL1Info.matched = cms.InputTag("gtStage2Digis:Muon:RECO")
```
## for MkBatch ##
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
