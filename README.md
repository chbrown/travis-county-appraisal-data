## Appraisal data

The data in this folder was purchased from the [Travis Central Appraisal District](http://www.traviscad.org/) by me on 2015-06-23 for 80 USD.

Before purchasing, I inquired whether I could share the data with others. They responded:

> The export is public information

So I am publishing it here for easier access to future users.


## Received files

The Travis Central Appraisal District Records Coordinator uploaded 3 files to an FTP server (running `pure-ftpd`) that I started on a Digital Ocean droplet for the sole purpose of this transaction.

| Original filename                                                   | File size | MD5 checksum                     |
|:--------------------------------------------------------------------|----------:|---------------------------------:|
| `2015-06-23_005220_APPRAISAL R&P ALLJUR AS OF 2015 PRELIMINARY.zip` | 245489827 | 29b6970de527d400b06d516dc0111d8e |
| `Shapefiles_Future_Year_2015-06-01.zip`                             | 195657257 | 085d9206e628d5927e282e81dff1c547 |
| `Standard Layouts & Codes.zip`                                      |   4487862 | f15ce956cf140435d1feb08d89586fde |

## Extracted contents

**`2015-06-23_005220_APPRAISAL R&P ALLJUR AS OF 2015 PRELIMINARY.zip`** expands to nearly 12 GB and contains these files:

| Filename                   | File size  |
|:---------------------------|-----------:|
| `ABS_SUBD.TXT`             |    1109576 |
| `AGENT.TXT`                |     466640 |
| `APPR_HDR.TXT`             |        246 |
| `ARB.TXT`                  |   10272012 |
| `ARBITRATION.TXT`          |        952 |
| `COUNTRY.TXT`              |      13965 |
| `ENTITY.TXT`               |       3933 |
| `IMP_ATR.TXT`              |  201853068 |
| `IMP_DET.TXT`              | 1696625424 |
| `IMP_INFO.TXT`             |   39719328 |
| `LAND_DET.TXT`             |   73856646 |
| `LAWSUIT.TXT`              |     172431 |
| `MOBILE_HOME_INFO.TXT`     |   13222740 |
| `PROP.TXT`                 | 3589864128 |
| `PROP_ENT.TXT`             | 6331668303 |
| `STATE_CD.TXT`             |       5922 |
| `TOTALS.TXT`               |     387504 |
| `Transfer Tape Totals.pdf` |     582412 |
| `UDI.TXT`                  |          0 |

I have moved these into [`roll-extract/`](roll-extract/) and bzip2'ed all files over 100 KB, achieving a compression ratio of nearly 99%.

**`Shapefiles_Future_Year_2015-06-01.zip`** expands to 663 MB, comprising 92 files, which form 23 groups of `.{shx,shp,prj,dbf}` files.

I have moved these into [`gis/`](gis/) and tarballed them into 23 `.tar.bz2` files, for a compression ratio of nearly 71%.

**`Standard Layouts & Codes.zip`** comprises the documentation for this dataset.

I have moved these files into [`docs/`](docs/) but otherwise left them untouched.
