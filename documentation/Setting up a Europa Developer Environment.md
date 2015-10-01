# Setting Up a Europa Developer Environment
To provision a Europa developer environment there are 2 options available:

## 1. Import a pre-built image from the Environments Management share
Currently pre build Europa images are kept in the following location:
https://webfiles.sivdi.uk/files

You will need to request access to the share by sending an email to the following email address:
**emsupport@atos.net  **


1. Once you have been granted access to the share go to the Europa directory and download the following 12 zip files:
| File Name	 | Size on Disk |
|--------|--------|
|europa.7z.001	|	734,003,200| 
|europa.7z.002	|	734,003,200 
|europa.7z.003	|	734,003,200 
|europa.7z.004	|	734,003,200 
|europa.7z.005	|	734,003,200 
|europa.7z.006	|	734,003,200 
|europa.7z.007	|	734,003,200 
|europa.7z.008	|	734,003,200 
|europa.7z.009	|	734,003,200 
|europa.7z.010	|	734,003,200 
|europa.7z.011	|	734,003,200 
|europa.7z.012	|	249,943,996 

1. Unzip the files to a local directory on your computer using the 7-Zip utility by right clicking the europa.7z.001 file and selecting Extract to “europa\”
if you do not have a local copy of 7-zip on your desktop, the product can be downloaded from the following location:
http://www.7-zip.org/download.html
1. The unzipped Europa image should produce a single file called Europa.ova. Using an MD5 checksum utility ensure both the downloaded zip files and the unzipped  ova file have the following MD5 checksums:
| Checksum | File Name |
|--------|--------|
|aafabac3177e809b432774e8c5c65dd6 |	europa.ova |
|9b3d6658034459a4e041d2a649218f55 |	europa.7z.001|
|2246I9b20330f603031acb037bd700cdd |europa.7z.002|
|ff3bf05dfedc35c8db056dc78b7a5555 |	europa.7z.003|
|a20842b33950e9ff3990022202a15e3a |	europa.7z.004|
|8b476970b765ff900bed6292a615f7e8 |	europa.7z.005|
|69d7c969cc48ee748ea96cb48900cc9a |	europa.7z.006|
|f2d873905e94d73aeeab692c9b0e8916 |	europa.7z.007|
|e486b24026b4572166748c06c838e034 |	europa.7z.008|
|73be3d34865b476504b5dccfa66410d4 |	europa.7z.009|
|821ac4f5150626fdc3e3779bca1b45c3 |	europa.7z.010|
|268be0178aa9bfdd2a0e7ee0d679279c |	europa.7z.011|
|ea339dac9a7d4c50c6489d3b614775d8 |	europa.7z.012|

1. Install VirtualBox to your computer using the following work instruction
https://sp.myatos.net/si/UKI/tp/Digital/Documents/012%20-%20PAMM%20and%20JAMM%20-%20Agile%20and%20CI%20tooling/How%20to%20set%20up%20VirtualBox.docx

1. Upload the Europa.ova file to VirtualBox using the previously unzipped to local disk as per the following work instruction
https://sp.myatos.net/si/UKI/tp/Digital/Documents/012%20-%20PAMM%20and%20JAMM%20-%20Agile%20and%20CI%20tooling/How%20to%20run%20a%20virtual%20environment%20on%20VirtualBox.docx


- - -


## 2.	Build image from scratch using DevOps scripts
Alternatively you may wish to build the image from scratch using the pre-configured Ansible scripts.
2.  Set up your Windows laptop with the pre-requisite build tools using the following work instruction
https://sp.myatos.net/si/UKI/tp/Digital/Documents/012%20-%20PAMM%20and%20JAMM%20-%20Agile%20and%20CI%20tooling/Windows%20Virtual%20Box%20Build%20Environment.html
 
2. Download the latest build scripts from NEUS project on GITHub
https://github.com/gatblau/neus

2. Navigate to the root directory of the Neus repository in Cygwin and execute the following command
sh build.sh
2. Select option '**e**'

    [a] PAMM Development (Virtual Box) Vagrant Base Box - No UI"
    [b] PAMM Development (Virtual Box) - Desktop UI"
    [c] PAMM Development (VMWare) - CI"
    [d] PAMM Development (VMWare) - Server UI"
**    [e] Europa Development (Virtual Box) - Desktop UI"**
    [e] CI Compact (VMWare) - No UI"
    [x] Refresh downloaded packages"
    [q] Quit Menu"
`


## 3.  	Installed Software on Europa
The following applications will be found in the newly built Europa environment

•	Centos 7.1
•	Java JDK 1.8
•	Vagrant
•	Google Chrome
•	SBT(Scala Build Tool)
•	Packer
•	IntelliJ Ultimate Edition
•	Eclipse
•	MySQL Workbench
•	Git
•	Groovy
•	Gradle
•	Maven
•	Haroopad
•	RoboMongo
•	Docker
•	NodeJS


#####3.1 PAMM

#####3.1 JAMM



## 4.	Europa Users & Accounts
|Application| Username | Password |
|-----------|----------|----------|
|Operating System/root	|root|	Passw0rd!|
|Operating System/user account|	vagrant|	vagrant|

