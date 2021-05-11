# app-ctf2fif

Convert ctf files into fif format using `bl2bids` tool and [`mne_bids`](https://mne.tools/mne-bids/dev/index.html).

# app-ctf2fif documentation

1) Convert ctf files into fif format
2) Input files is a MEG file in `.ctf` format
3) Input parameters are used to set the BIDSpath, they are:
    * subject: `str` or `None`, the subject ID. Corresponds to “sub”,
    * session: `str` or `None`, the session for a item. Corresponds to “ses”,
    * task: `str` or `None`, the task for a item. Corresponds to “task”,
    * run: `str` or `None`, the run number for this item. Corresponds to “run”,
    * acquisition: `str` or `None`, the acquisition parameters for the item. Corresponds to “acq”, 
    * processing: `str` or `None`, the processing label for this item. Corresponds to “proc”,
    * recording: `str` or `None`, the recording name for this item. Corresponds to “rec”,
    * space: `str` or `None`, the coordinate space for an anatomical or sensor position files. Corresponds to “space”, 
    * suffix: `str` or `None`, the filename suffix. This is the entity after the last _ before the extension. 
 
### Authors
- [Aurore Bussalb](aurore.bussalb@icm-institute.org)

### Contributors
- Soichi Hayashi
- Giulia Berto

### Funding Acknowledgement
brainlife.io is publicly funded and for the sustainability of the project it is helpful to Acknowledge the use of the platform. We kindly ask that you acknowledge the funding below in your code and publications. Copy and past the following lines into your repository when using this code.

[![NSF-BCS-1734853](https://img.shields.io/badge/NSF_BCS-1734853-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1734853)
[![NSF-BCS-1636893](https://img.shields.io/badge/NSF_BCS-1636893-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1636893)
[![NSF-ACI-1916518](https://img.shields.io/badge/NSF_ACI-1916518-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1916518)
[![NSF-IIS-1912270](https://img.shields.io/badge/NSF_IIS-1912270-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1912270)
[![NIH-NIBIB-R01EB029272](https://img.shields.io/badge/NIH_NIBIB-R01EB029272-green.svg)](https://grantome.com/grant/NIH/R01-EB029272-01)

### Citations
1. Avesani, P., McPherson, B., Hayashi, S. et al. The open diffusion data derivatives, brain data upcycling via integrated publishing of derivatives and reproducible open cloud services. Sci Data 6, 69 (2019). [https://doi.org/10.1038/s41597-019-0073-y](https://doi.org/10.1038/s41597-019-0073-y)
2. Appelhoff, S., Sanderson, M., Brooks, T., Vliet, M., Quentin, R., Holdgraf, C., Chaumon, M., Mikulan, E., Tavabi, K., Höchenberger, R., Welke, D., Brunner, C., Rockhill, A., Larson, E., Gramfort, A., & Jas, M. MNE-BIDS: Organizing electrophysiological data into the BIDS format and facilitating their analysis. Journal of Open Source Software, 4:1896 (2019). [https://doi.org/10.21105/joss.01896](https://doi.org/10.21105/joss.01896)

## Running the App 

### On Brainlife.io

This App is still private on Brainlife.io.

### Running Locally (on your machine)

1. git clone this repo
2. Inside the cloned directory, create `config.json` with the same keys as in `config.json.example`.

```json
{
  "fif": "rest1-raw.fif"
}
```

3. Launch the App by executing `main`

```bash
./main
```

## Output

The output file is a MEG file in `.fif` format.
