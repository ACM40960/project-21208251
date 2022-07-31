## An Investigation into Global Climate Variables and the Key Determinants of Global Warming


### 1. Intended Use 🤝

The aim of this project is to conduct an investigation into the key determinants of global warming, with a focus on global climate variables. To aid with the investigation we have downloaded temperature, precipitation and carbon dioxide data from sources indicated below and made use of the Wolfram Knowledgebase. All analysis of data has taken place within Mathematica.

###  2. Mathematica Installation 📦 📂

#### Introduction

Mathematica is a computing system which is favoured across many disciplines from geo-spatial mapping to general relativity for its excellence in data science, visualisation and image processing. It is a high-level programming language, making prototyping solutions to a variety of problems straight-forward.

#### Institution License

You can find out if your academic institution holds a site license to Mathematica by following the link the the [Mathematica homepage](https://www.wolfram.com/mathematica/).
1. Follow the banner to find out if you already have access to Wolfram tech through your institution.
2. Enter the email address that is associated with your organisation and tick the box to agree to the retention of personal data.
3. Assuming eligibility, you will be prompted to confirm status at the organisation and brought to a software download page.

![image](https://user-images.githubusercontent.com/60405870/181994454-1c5c3f40-ea87-4553-a6c1-9dc94f1ab1a3.png)
![image](https://user-images.githubusercontent.com/60405870/181994582-3907f6c3-e576-4469-9237-802dd11dc9f1.png)

UCD's sotware download page provides the following instructions for first time download of Mathematica software.

You will be required to 
- Check your email and click the link to validate Wolfram ID.
- Fill out the Wolfram Home Use Request Form if prompted to do so. This will request an activation key for a single machine.
- You will then receive an email from Wolfram with the Activation Key and a link to download the installer.
- Follow the link to sign into the Wolfram User Portal.
- Download and run the installer.
- Enter the Activation Key when prompted to do so.

#### General User

If you cannot access Wolfram Mathematica through your Institution, you can buy a licence via their [website](https://www.wolfram.com/mathematica/pricing/). On this page you may choose your subscription plan. However, note there is a fee attached to general licenses according to which package the user chooses. A video tutorial posted by the Wolfram community on how to download the software for Windows and Mac can be found [here](https://community.wolfram.com/groups/-/m/t/2332560?sortMsg=Replies).

[(Back to top)](#an-investigation-into-global-climate-variables-and-the-determinants-of-global-warming)



### 3. Data 📊 📈 

The user can choose to download the files directly from the pages linked by following the instructions given below to the precise data-sets, or they can choose to download the data-sets included within this repository, along with the google drive links which have been provided for the two biggest files. In both cases please note:

1. All data-sets are updated by the associated body regularly, meaning it is likely that there will be some additional data observations added to the data-set when the user downloads the data-file from the parent directory. This should not create a problem when running the Mathematica document as steps have been taken to overcome any issues this might cause. However, lines of text within the Mathematica document referring to size and dimensions of data-sets may be off.

2. Dowloading the data-files directly from this repository (and the google drive) means the user will have access to the exact same data-files used by the authors in their analysis. 

Links and instructions are provided below to download the current versions of each of these file. Code will run with either verion of the files, but outputs and comments may not be accurate for the updated files.

#### Temperature Data 🌡️ ❄️ 🔥

The [temperature data ](https://www.metoffice.gov.uk/hadobs/hadcrut5/data/current/download.html )
obtained from Met Office Hadley Centre observations datasets, where we downloaded 3 files:

1. HadCRUT5 analysis time series: ensemble means and uncertainties: Summary Series Global Monthly NetCDF;
2. HadCRUT5 analysis time series: ensemble members: Ensemble Series Global Monthly NetCDF;
3. HadCRUT5 analysis gridded data: additional fields: Ensemble mean NetCDF.

The first two files are available to download via the repository, with the third available via this [google drive](https://drive.google.com/file/d/1m7OuZfm4OIvqxntjOL4wOGmC8j6YVN0E/view?usp=sharing).

![image](https://user-images.githubusercontent.com/60405870/181915878-c8c1037c-0570-4d1c-9007-99b6ca751970.png)

![image](https://user-images.githubusercontent.com/60405870/181915981-1f0f87f2-8767-49b3-8359-50ffc74eacb2.png)

[(Back to top)](#an-investigation-into-global-climate-variables-and-the-determinants-of-global-warming)

#### Precipitation Data ☔ 🌀 ⛈️

The [precipitation data](https://downloads.psl.noaa.gov/Datasets/ghcngridded/)
is available through the National Oceanic and Atmospheric Administration Physical Sciences
Laboratory, and is produced under the Global Historical Climatology Network. 
The associated dataset is the Precipitation Anomaly Dataset, and can also be obtained via this [google drive](https://drive.google.com/file/d/1PYcMpkWQY_o181U9VdLMM5i42gNjIzYd/view?usp=sharing) link, or the link to the page above.

![image](https://user-images.githubusercontent.com/60405870/181916247-9e4269f5-2747-4bd1-8157-8f12b6bc42c7.png)

[(Back to top)](#an-investigation-into-global-climate-variables-and-the-determinants-of-global-warming)

#### Carbon Dioxide (CO$_2$) ✈️ 🚛 🏭 

Carbon dioxide data is freely available through the Global Monitoring Laboratory (GML) of the National Oceanic and Atmospheric Association (NOAA). The initial lines within each dataset contain meta-data on usage. The [CO2](https://gml.noaa.gov/aftp/products/trends/co2/) directory contains 

From here, we have made use of the three files:

1. Estimated CO2 Daily Global Seasonal Cycle and Trend (ppm)

* file name co2_trend_gl.csv

2. CO$_2$ Global Annual Mean Estimates at Mauna Loa, Hawaii.

* file name co2_annmean_mlo.csv

3. CO$_2$ Global Monthly Estimates at Mauna Loa, Hawaii.

* file name co2_mm_mlo.csv

Each of these files are also available to download via the repository. 
![image](https://user-images.githubusercontent.com/60405870/181995301-0a1cd818-31da-40e0-9e22-81c0ed7facc5.png)


[(Back to top)](#an-investigation-into-global-climate-variables-and-the-determinants-of-global-warming)

### 4. Running the notebook 🏃‍♀️ 🖥️ 

#### Downloading and opening the notebook

To run the notebook, download the ACM40960_21208251_16310126.nb included within this repository along with all prescribed data-sets. There should be 7 data-sets downloaded and included in the same folder as the Mathematica notebook. Opening Mathematica on your desktop should open on the following page:

![image](https://user-images.githubusercontent.com/60405870/181854711-00dee655-c37b-4269-975c-086cbe729d64.png)

Open the Mathematica notebook file. We recommend the user evaluate the notebook before expanding sections. Doing so takes approximately 2 minutes 24 seconds. The Evaluate Notebook option is included under the the evaluation tab:

![image](https://user-images.githubusercontent.com/60405870/181855350-fdfb1e80-435b-4ee1-be20-a5cf0ba6ca86.png)

Please note that the user can choose to run the notebook section by section, but should bear in mind the notebook is organised using a top-down approach. Data importation and cleaning in preliminary sections informs analysis and organises data in sections to follow.

#### Sections of the notebook 🔢

The notebook is organised into six sections across 
1. Importing Data;
2. Data Cleaning;
3. Overview Plots;
4. Norway and Libya Case Studies;
5. Linear Modelling;
6. Carbon Dioxide.

Sections can be expanded in a few different ways. By clicking the section expansion button the section is opened:

![image](https://user-images.githubusercontent.com/60405870/181996215-3151a25d-47d4-4bc6-85c9-372d45e17587.png)

The user can also choose to use the keyborad shortcut `cmd + '` or `ctrl + '` on a mac or windows system. Within each section there are detailed subsections which can be opened and closed in the same way.

[(Back to top)](#an-investigation-into-global-climate-variables-and-the-determinants-of-global-warming)

### 5. Authors 👩‍🔬 👩‍🔬
 
Eilish Clune & Megan Farrell (21208251, 16310126).

[(Back to top)](#an-investigation-into-global-climate-variables-and-the-determinants-of-global-warming)
