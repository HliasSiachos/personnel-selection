# Code for the paper 'Making personnel selection smarter through wordembeddings: A graph-based approach'

This repository hosts code for the papers:
* []() - [Download]()

![image1](https://github.com/imis-lab/journal/blob/develop/GraphOfDocs_Representation/images/graph-of-docs.jpg)

## Datasets
Available in [this link]()

## Test Results
Edit `experiments.ipynb`.

## Installation
**Prequisites:**
* `Windows 10` 64-bit / Debian based `Linux` 64-bit.  
* `Python 3` (min. version 3.6), `pip3` (& `py` launcher Windows-only).  
* Working `Neo4j` Database (min. version 4.1.2).  

### Windows 10
Download the project from the green button above, unzip it,  
and then open a cmd terminal to this folder and type `pip3 install -r requirements.txt`.  
This command will install the neccessary `Python` libraries\* to run the project.  

### Debian Based Linux
We ran the following commands to update `Python`, `git`,  
clone the project to a local folder and install the necessary `Python` libraries\*.
```bash
sudo apt install python3.6
sudo apt install git-all
git clone https://github.com/imis-lab/personnel-selection
cd personnel-selection
pip3 install -r requirements.txt
```
*\* Optionally you could create a virtual environment first,*  
*\* to isolate the libraries from your python user install.*  
*\* However the setup script doesn't downgrade existing libraries,*  
*\* so there's zero risk in affecting your local user install.*  

## Database Setup (Windows / Linux)
Create a new database from the `Neo4j` desktop app using 4.1.2 as the min. version.  
Update your memory settings to match the following values,  
and install the following extra plugins as depicted in the image.
![image2](https://github.com/imis-lab/journal/blob/develop/GraphOfDocs_Representation/images/settings.jpg)
*Hint: if you use a dedicated server that only runs `Neo4j`, you could increase these values, 
accordingly as specified in the comments of these parameters.*

Run the `GraphOfDocs_Representation.py` script which will create thousands of nodes, 
and millions of relationships in the database.  
Once it's done, the database is initialized and ready for use. 

## Running the app
You could use the `Neo4j Browser` to run your queries, 
or for large queries you could use the custom visualization tool  
`visualize.html` which is located in the `GraphOfDocs_Representation` Subdirectory.

## Contributors
* Nikolaos Giarelis (giarelis@ceid.upatras.gr)
* Nikos Kanakaris (nkanakaris@upnet.gr)
* Ilias Siachos (ilias.siachos@ac.upatras.gr)
* Nikos Karacapilidis (karacap@upatras.gr)
