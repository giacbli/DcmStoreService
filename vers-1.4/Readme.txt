DcmStoreService (Dicom Store Service)
Author: Giacomo Belli - 2016
Health Physics Unit - AOU Careggi
Florence - Italy

Previous releases:

September 2023 - vers. 1.1

A lightweight and efficient Dicom server to receive and store medical images such as CT, MRI, DX, MG, XRF, XA, NM, PET, US etc., 
as well as Structured Radiation Dose Reports (non-image SOP classes).
The application (C++ compiled) implements the Dicom Storage SCP class and runs as an automatic MS Windows service (x86/x64 platform Win 7-8-10-11).

May 2024 - vers. 1.3

New features available in this release:
- Possibility to increase the maximum number of worker threads to improve performance in case of concurrent client connections
- An option that allows image names to be indexed based on the Dicom Image Number tag, as an alternative to the cryptic naming of the image's SOPInstanceUID;
- Capability to create the DICOMDIR directory file for each study stored. 


Latest release, July 2025 - vers. 1.4

New features available in this  release:
- It is now possible to manage a custom list of DICOM images and non-image DICOM objects, read from a configuration file. It also offers a choice of transfer syntaxes among those provided and negotiable with the SCU client application. If the configuration file is not found, the storage server works regularly for a set of default Dicom SOP classes.
- A new option is available to let storing of any Structured Report file in a single folder or in a tree structure of subfolders.
- The system tries to intercept anomalous situations in which the images from different acquisitions, but belonging to the same study, are sent with the same serial number and instance index as the previously stored images. A filename splitting mode (numbering extension) has been implemented to prevent overwriting during archiving. This abnormal situation of possible overwriting should not occur if files are named using Dicom unique identifiers (UID).

Please read file ReadMe_DcmStore.pdf for more details and installation instructions.

