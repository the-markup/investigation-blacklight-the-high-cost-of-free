## The High Privacy Cost of a ‘Free’ Website

This repository contains the data analysis described in our [methodology](https://themarkup.org/blacklight/2020/09/22/how-we-built-a-real-time-privacy-inspector#limitations) and our story [The High Privacy Cost of a ‘Free’ Website](https://themarkup.org/blacklight/2020/09/22/blacklight-tracking-advertisers-digital-privacy-sensitive-websites).

### Installation

Make sure you have Python 3.6+ installed.

Install Python packages:
pip install -r requirements.txt

### Data

Please download the data using the `download-data.sh` script.

All reports generated for this analysis were done so using the `blacklight-reporter`please refer to its [README](https://github.com/the-markup/blacklight-reporter) for more information about the indivudual reports.

The data folder is organzied as follows:<br>

| Folder                                               | Description                                                                                                                                                                                              |
| :--------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `data/tranco-V3Kn-100k.txt`                          | The unique Tranco 100k URL list used for this scan. More info [here](https://tranco-list.eu/list/V3KN/full)                                                                                              |
| `data/reports/tranco-V3Kn-100k`                      | The reports generated from the scan of the `tranco-V3Kn-100k.txt` list.                                                                                                                                  |
| `data/reports/local-urls-for-experiment-2020-07-29`  | The local reports generated from the local vs remote experiment described in the [methodology](https://themarkup.org/blacklight/2020/09/22/how-we-built-a-real-time-privacy-inspector#limitations).      |
| `data/reports/remote-urls-for-experiment-2020-07-29` | The remote reports generated from the local vs remote experiment described in the [methodology](https://themarkup.org/blacklight/2020/09/22/how-we-built-a-real-time-privacy-inspector#limitations).     |
| `data/story-inspections`                             | The `blacklight-collector` inspections for the websites mentioned in our [investigation](https://themarkup.org/blacklight/2020/09/22/blacklight-tracking-advertisers-digital-privacy-sensitive-websites) |

## Notebooks

### 0-100k-scan.ipynb

This notebook contains the analysis for the reports generated from the 100,000 most popular website. This includes the statistics used in our [story](https://themarkup.org/blacklight/2020/09/22/blacklight-tracking-advertisers-digital-privacy-sensitive-websites) and [Show Your Work](https://themarkup.org/blacklight/2020/09/22/blacklight-tracking-advertisers-digital-privacy-sensitive-websites). We scanned the most popular 100,000 websites as defined by the Tranco list [^ 1](https://tranco-list.eu/list/V3KN) created on 29 August 2020.

### 1-local-vs-remote-experiment

This notebook contains the aggregate statistics for the experiment defined in the our [Show Your Work](https://themarkup.org/blacklight/2020/09/22/how-we-built-a-real-time-privacy-inspector#survey)

### Licensing

Copyright 2020, The Markup News Inc.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

    Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.

    Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

    Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
