# Filelists for PPG04 
- These filelists only work on SDCC. 

## Simulation
- *HIJING* : 
    - `sim_hijing_nop` : Central sPHENIX simulation of MB HIJING (0-20 fm) with no puileup (Type 4, run 19, -nop)
    - `sim_hijing_pileup` : Central sPHENIX simulation of MB HIJING (0-20 fm) with AuAu 50 kHz pileup (Type 4, run 19, -pileup)

* All HIJING simulation filelists are generated for DST_CALO_CLUSTER, DST_GLOBAL, DST_MBD_EPD

- *PYTHIA* : 
    - `sim_jet10_embed` : Central sPHENIX simulation of PYTHIA dijets with ${p}_{T}^{\textrm{min}} = 10$ GeV/c embedded in MB HIJING (0-20 fm) AuAu 50 kHz pileup (Type 12, run 19, -embed)
    - `sim_jet30_embed` : Central sPHENIX simulation of PYTHIA dijets with ${p}_{T}^{\textrm{min}} = 30$ GeV/c embedded in MB HIJING (0-20 fm) AuAu 50 kHz pileup (Type 11, run 19, -embed)
    - `sim_jet10_pp` : Central sPHENIX simulation of PYTHIA dijets with ${p}_{T}^{\textrm{min}} = 10$ GeV/c with no pileup (Type 12, run 19, -nop)
    - `sim_jet30_pp` : Central sPHENIX simulation of PYTHIA dijets with ${p}_{T}^{\textrm{min}} = 30$ GeV/c with no pileup (Type 11, run 19, -nop)

* All PYTHIA simulation filelists are generated for DST_CALO_CLUSTER, DST_GLOBAL, DST_MBD_EPD, DST_TRUTH_JETS

## Data
* The run number used for PPG04 is 23745. The most current production for run 2023 calo data is build `ana412` production `2023p015`. The filelists can be genrated with the `CreateDataLists.py` script like this:
```bash
    python3 CreateDataLists.py -r 23745 -b ana412 -d 2023p015
```
