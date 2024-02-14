# bluehill-universal-overlay-tool
Tool to take multiple raw data export data files from Instron Bluehill Universal software (in .csv format) and overlay them on a single stress strain axis. 

Running the script will launch a GUI prompting user to select a folder containing raw data .csv files from Instron Bluehill Universal, as well as the gauge length of Instron machine and denier of tensile sample. User should populate the chosen folder beforehand with the desired files - each file should represent 1 curve/specimen of interest. Currently there is no functionality to "average" individual specimens (from the same sample) into one representave file.

Program exports .xlsx file with single stress strain chart and data from all imported .csv files. Chart can then be further formatted within Excel to suit the user's needs, avoiding knowledge of a programming language as a barrier for chart customization. 

Note: Ensure that the export .csv file from Bluehill is in the following format and units. See sample_csv_exports for examples.

| Time | Displacement | Force  |
|------|--------------|--------|
| (s)  | (in)         | (lbf)  |
| 0    | 0            | 0      |
| 0.02 | 0.0014       | 0.0081 |

# INSTALLATION:
Ensure you have python3 installed on your system. (https://wiki.python.org/moin/BeginnersGuide/Download)

## Install required modules
Use pip package installer
```bash
pip install -r PATH/TO/requirements.txt
```
