DcmStoreService (Dicom Store Service)
Author: Giacomo Belli - 2016
Health Physics Unit - AOU Careggi
Florence - Italy

September 2023 - vers. 1.1

A lightweight and efficient Dicom server to receive and store medical images such as CT, MRI, RX, MG, XRF, XA, NM, PET, SR, US etc., 
as well as Structured Radiation Dose Reports.
The application (C++ compiled) implements the Dicom Storage SCP class and runs as an automatic MS Windows service (x86/x64 platform Win 7-8-10-11).

Please read file ReadMe_DcmStore.pdf for more details and for the installation instructions.

Latest release, May, 2024 - vers. 1.3

New features available in this  release:
- Possibility to increase the maximum number of worker threads to improve performance in case of concurrent client connections
- An option that allows image names to be indexed based on the Dicom Image Number tag, as an alternative to the cryptic naming of the image's SOPInstanceUID;
- Capability to create the DICOMDIR directory file for each study stored. 




