# CLIP - We live in a world of rising seas 

## Background on this CLIP

Sea level rise is one of the best known and already most visible signs of climate change in many regions of the world. For this reason, the "classic curve" of the rise is presented in this CLIP. In contrast to other representations, however, a classification is to be made here along comments. These can be explanations of the curve itself (as currently shown), dates of climate conferences or other temporal classifications.

## Data Sources

The CLIP uses the following dataset:

- [ESA Sea Level CCI: Oceanic Indicators of Mean Sea Level Changes (MSL), Version 2.0](https://catalogue.ceda.ac.uk/uuid/3ac333b828b54e3495c7749f5bce2fe3), 
  Cate dataset identifier: `esacci.SEALEVEL.mon.IND.MSL.multi-sensor.multi-platform.MERGED.2-0.r1`.

## Data Preparation

### Description

Data preparation comprises the following steps:

* Opening the Sea Level CCI dataset `esacci.SEALEVEL.mon.IND.MSL.multi-sensor.multi-platform.MERGED.2-0.r1`.
* Select time-series variable "Global mean sea level variations" (`global_msl`).
* Convert time-series into a data frame and save a CSV file `data/global_msl.csv`. 
  The units are meters.

### One-time script setup

If you do not have a Cate account yet, please visit [Cate App](https://cate.climate.esa.int/), select **Cate Cloud Service** and register. 
Using the Cate credentials, login to the [Cate JupyterLab](https://cate-lab.brockmann-consult.de/). 
From the JupyterLab's **Launcher**, open a **Terminal** window and type

```bash
cd ~/work
git clone https://github.com/trevalabs/pytrevalabs.git
git clone https://github.com/trevalabs/clip_02_we_live_in_a_world_of_rising_seas.git
```

Note you can also use the JupyterLab's **Git** extension (left side bar) to clone the repos.

### Running the script

In JupyterLab's **File Browser** navigate to `/clip_02_we_live_in_a_world_of_rising_seas/scripts/dataprep` and open
the Notebook [extract-sea-level.ipynb](scripts/dataprep/extract-sea-level.ipynb) and run it.

To stay in sync with the repos, open a **Terminal** window and

```bash
cd ~/work/pytrevalabs
git pull --rebase
cd ~/work/clip_02_we_live_in_a_world_of_rising_seas.git
git pull --rebase
```

Note you can also use the JupyterLab's **Git** extension (left side bar) to update the repos.


## Creating Visualizations
[STEP BY STEP DESCRIPTION ON WHAT THE DATA PROCESSING PROCESS. SHOULD BEGIN WITH A SHORT SUMMARY OF THE OVERALL PROCESS]
Work in Progress

## CLIP URL (Result)
https://www.datawrapper.de/_/kQI21/

## CREDITS & LICENSE
- Idea by: [Philipp Eales](http://www.planetaryvisions.com/index.php)
- Processing Scripts by: [Brockmann Consult](https://www.brockmann-consult.de/)
- Visualization by: [Ubilabs](https://ubilabs.com/de)

The code in this repository is published under [CC BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/)
