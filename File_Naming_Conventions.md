# File Naming Conventions
## Abstract
This documents is intended to be a central guide for the naming and management of files for this project. With such a large number of overlapping variables and stakeholders, it's crucial that we appropriately title files such that there can be no mistake of their origin or their purpose. 

## Terms
For this project, I will be using the three **A**s to make distinction between file types. The three **A**s are **A**rchive, **A**sset and **A**ccess. 

### Archive copies
The archive copy is always the best copy of an available item. This could be a raw scan of a negative, a digital raw file from a digital camera, an original video stream digitized from hard media or an unaltered scan of paper ephemera. The archive copy is the most important copy, as it contains the most information. These copies are rarely made available to the public, and exist primarily for internal use.

### Asset copies
The asset copies of a file are versions of the archive copy which have been tailored to specific uses. Asset copies retain as much information as possible but may have their file-type, resolution and other attributes changed to match the use case. Sometimes the alterations include artistic decisions such as cropping or color changes. Asset copies are not as crucial as archive copies, but very important to maintain the integrity of a given project and should be treated as such. They should be stored according to their end use (i.e. asset files for web publishing stored in "web" folder, asset files for React stored in "React" folder and so forth)

### Access copies
The access copy of a file is typically a compressed, lossy version of the archive copy. The purpose of access copies is to provide a small and lightweight file which can be used as preview, or to share with clients/stakeholders without giving them direct access to publishable files. Access copies are meant to be easy to email and recall.

## How does this look in practice?

If we were dealing with a hypothetical file from ASM's photographic collection with the accession number **12345**, the file names could look as follows;

  - **archive copy:** 12345_scan.tif
  - **an asset copy for Unity:** 12345_ast_unity.png
  - **an asset copy for React:** 12345_ast_react.png
  - **an access copy to send to stakeholder:** 12345_acc.jpg

For files we are generating specifically for this project such as original scans of outside materials, the filenames will originate 
