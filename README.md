# WEAP: Whole Exome Analysis Pipeline


Operating system(s): Ubuntu 18.04 or higher.


Programming language: Bash.


Other requirements: Java 1.3.1 or higher, Python3, GLIBC 2.28 or higher.


## 1.Downloading WEAP

i.	Install git using:


      sudo apt -y install git


ii.	Change the current directory to Desktop:


      cd  ~/Desktop


iii.	Download WEAP using git:


       git clone https://github.com/ranjanjs34/weap.git


iv.	After downloading, enter into the WEAP:


       cd WEAP
       
       
NOTE: Advanced users may keep WEAP in any convenient location. 


## 2.Setting Up WEAP:


Add execution permission to binary files configure and reference:


       sudo chmod  +x ./ configure
       sudo chmod  +x ./ reference



## 3.Downloading prerequisite tools [One Time]


To download the prerequisite tools, run the configure as :


       ./configure


Enter the directory address where it download the pre-requisite tools:
for example: /home/$USER/Desktop


There should not be any ‘/’ at the end of the directory address. 



This Script will automatically download and install the required tools add to path so that WEAP can recognize the internal commands. As ANNOVAR cannot be distributed, users need to download the ANNOVAR from the ANNOVAR website after registration. Please download the ANNOVAR from https://www.openbioinformatics.org/annovar/annovar_download_form.php manually by registering, unzip  and keep  it in Tool directory as 'annovar'.



## 4.Downloading Reference Data:


       ./reference
This will download the reference genome, Variants with Allele frequency from genomAD project, dbSNP data from gatk bundle and datasets from ANNOVAR web resource to annotate the variants. 






## 5.How to Run WEAP for variant calling (WEAP will guide the users at each step for the input):

    
      ./WEAP
