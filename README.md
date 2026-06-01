# DcmStoreService  (Dicom Storage Service)

A lightweight and efficient Dicom server to receive and store medical images such as CT, MRI, RX, MG, XRF, XA, NM, PET, US etc., as well as Structured Radiation Dose Reports (non-image SOP classes).
The application (C++ compiled) implements the Dicom Storage SCP Service and runs as an automatic MS Windows service (x86/x64 platform Win 7-8-10-11).

### Some features:
- Can receive medical images and structured reports on radiation dose in Dicom format from company PACS and radiology equipment

- Multithreaded architecture to handle concurrent client connections

- Creates a tree-architecture folder system (based on study ID or patient name) for archiving study images. Cabability to create the DICOMDIR directory file.

- Some simple scripts and files are provided to manage and configure the application as automatic MS Windows system service (24 hrs)


**Please read the file ReadMe_DcmStore.pdf for more details and for the installation instructions.**
   

First release available, Sep, 2023 - vers. 1.1

### Updates:

##  Vers. 1.3, May, 2024
### New features available in this release:
- Possibility to increase the maximum number of worker threads to improve performance in case of concurrent client connections.
- An option that allows image names to be indexed based on the Dicom Image Number tag, as an alternative to the cryptic naming of the image's SOP Instance UID.
- Capability to create the DICOMDIR directory file for each study stored.

## Vers. 1.4, July, 2025
### New features available in this latest release:
- It is now possible to manage a custom list of DICOM images and non-image DICOM objects, read from a configuration file. It also provides a choice of transfer syntaxes among those negotiable with the SCU client application. Without this configuration file, the storage server still works normally for a set of default Dicom SOP classes.
- A new option is available to let storing of any Structured Report file in a single folder or in a tree structure of subfolders.
- This tool attempts to intercept anomalous cases where images from different acquisitions, but belonging to the same study, are sent with the same serial number and instance index as previously stored images. A filename splitting (numbering extension) mode has been implemented to prevent overwriting during archiving.

###

![Send-to-storage service-ultrasmall](https://github.com/giacbli/DcmStoreService/assets/15181782/d3c31ce8-046b-45f6-831f-87aec9ed98c1)




Author: Giacomo Belli -
Health Physics Unit – AOU Careggi
Florence - Italy
