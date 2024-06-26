# DcmStoreService  (Dicom Storage Service)

A lightweight and efficient Dicom server to receive and store medical images such as CT, MRI, RX, MG, XRF, XA, NM, PET, US etc., as well as Structured Radiation Dose Reports.
The application (C++ compiled) implements the Dicom Storage SCP Service and runs on computer as automatic MS Windows service (x86/x64 platform Win 7-8-10-11).

### Some features:
- Can receive medical images and structured reports on radiation dose in Dicom format from company PACS and radiology equipment

- Creates a tree-architecture folder system (based on study ID or patient name) for archiving study images

- Some simple scripts and files are provided to manage and configure the application as automatic MS Windows system service (24 hrs)


**Please read attached file ReadMe_DcmStore.pdf for more details and for the installation instructions.**
   

Previous release, Sep, 2023 - vers. 1.1


## Latest release, May, 2024 - vers. 1.3

### New features available in the latest release:
- Customizing the number of worker threads to improve performance for concurrent client connections.
- Indexing of image file names according to the Dicom Image Number tag, as an alternative to the cryptic name derived from the image's SOPInstanceUID.
- Capability to create the DICOMDIR directory file for each study stored. 




![Send-to-storage service-ultrasmall](https://github.com/giacbli/DcmStoreService/assets/15181782/d3c31ce8-046b-45f6-831f-87aec9ed98c1)




Author: Giacomo Belli -
Health Physics Unit – AOU Careggi
Florence - Italy
