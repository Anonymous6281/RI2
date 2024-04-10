# RI2
This is an anonymized, temporary repository for REAPER Infiller 2 for purposes of peer review. Following paper acceptance, this repository will be migrated to a permanent, non-anonymized repository.

REAPER Infiller 2 can be used on Windows, Mac, and Linux.

This anonymous video demonstrates the new feeatures introduced in REAPER Infiller 2: https://www.youtube.com/watch?v=6TJh3pHmjXY

**INSTALLATION INSTRUCTIONS**

***STEP 1***: Install REAPER (64-bit): https://www.reaper.fm/

***STEP 2***: Install a 64-bit version of python 3.9 or higher: https://www.python.org/downloads/

***STEP 3***: Configure REAPER to see your python installation. (In REAPER, this is in the Options > Preferences > Plug-Ins > ReaScript menu)

WINDOWS USERS: If all you want to do is use the model (e.g., you do not want to train it on your own files), you may skip to Step 5.

***STEP 4***: Install the following packages for your python installation: pytorch and transformers

-Pytorch installation: Go to https://pytorch.org/ to get the command you need to run, then run this command from the command line. You'll want the stable build for your OS, using the "Pip" package for Python (NOT Conda). If you have an NVIDIA card, it is recommended to install a CUDA version. Otherwise, install the CPU version, which is a bit slower. The command you use should start with something like "pip3 install torch..."

-Transformers installation: From the command line, run pip install transformers

***STEP 5***: Unzip one of the following releases to your REAPER folder. (To find your REAPER folder, from within REAPER go to Options > Show REAPER resource path in explorer/finder..., and then open the folder called Scripts.)

Users who did step 4 (including Windows users): Use [THIS DOWNLOAD](https://github.com/Anonymous6281/RI2/releases/download/v2.0.0/REAPER_Infiller_2.0.0.zip)

Windows users who skipped step 4: Download both of the following: [File 1](https://github.com/Anonymous6281/RI2/releases/download/v2.0.0/REAPER_Infiller_WIN_2.0.0.zip.001) [File 2](https://github.com/Anonymous6281/RI2/releases/download/v2.0.0/REAPER_Infiller_WIN_2.0.0.zip.002) (We had to split the Windows release into two files because of github's 2 GB per file size limitation. A single download file will be provided following paper acceptance.) Once both files are downloaded, with 7-zip, right click on the first file and click Open Archive, then drag everything in the archive to your REAPER folder.

Your files are in the right place if you have files like

YOUR_PATH_TO_REAPER\Scripts\REAPER_Infiller_v2\rpr_infiller_nn_server.py

and

YOUR_PATH_TO_REAPER\Effects\REAPER_Infiller_v2\RI Global Options

at this point.

***STEP 6***: Restart REAPER. Load the scripts into REAPER in the usual way: In REAPER, go to Actions > Show action list..., then click on New action > Load ReaScript..., and then open all scripts that start with "REAPER_". All other files are just helper files that these scripts need to run. Before you run any of the scripts, start the neural net server by running the rpr_infiller_nn_server.py file. The server window will need to remain open for the scripts to work.

***STEP 7***: Within REAPER, add the "Global Options for Infiller" fx your Monitor FX chain (view > Monitoring Effects). This fx will need to stay in your Monitor FX to have any effect. Add the "Track-Specific Generation Options" fx to any track that you want to set the infilling controls for before running one of the three REAPER scripts. ENJOY!

**NOTE**

The models in the release were trained only on public domain and permissively-licensed MIDI files. Please see the acknowledgements, disclaimer, and license in the download.

**HOW TO CITE**

Coming soon.
