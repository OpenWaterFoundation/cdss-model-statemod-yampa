# cdss-model-statemod-yampa #

[Colorado's Decision Support Systems (CDSS)](http://cdss.state.co.us) StateMod model dataset files for Yampa Basin.

This repository is an experiment created by the [Open Water Foundation](http://openwaterfoundation.org) to illustrate how a StateMod dataset can be maintained under version control using Git/GitHub.  The original version of the dataset was downloaded from the [CDSS StateMod website](http://cdss.state.co.us/Modeling/Pages/SurfaceWaterStateMod.aspx) on Aug 8, 2017.  It remains to be seen if this repository version is allowed to become the official master copy of the dataset.

## Repository Contents ##

The repository contains only the input files needed to create the Yampa Basin StateMod dataset:

* Data files used as input, such as time series that are from third parties and not found in HydroBase.
* Data Management Interface (DMI) software command files, such as for StateDMI and TSTool software.
* Documentation source files.

Dynamic files that can be created from the above source files or are created by running StateMod are not saved in the repository (.gitignore file is used to ignore):

* StateMod input files created by DMI programs.
* StateMod output files, such as reports and binary files.

Specific folders in the repository include the following.
It is convention that files are written into a data component folder and also
written to the main `StateMod` folder.
The latter is used to run the model.

* [Diversions]() - files related to direct diversions
* [DocsSW]() - Yampa River Basin Water Resources Planning Model User's Manual as PDF
* [Instream]() - files related to instream flow rights
* [Network]() - files related to model network
* [Reservoirs]() - files related to reservoirs
* [StateMod]() - folder where all generated files are placed as the complete dataset
* [StreamSW]() - files related to surface water streams

## Compatibility and Integration with other CDSS Models ##

The current dataset was created using the following software versions (versions assumed based on the file headers of the downloaded dataset).  It is generally safe to use later versions.

* HydroBase - 20160802
* StateDMI - ?
* TSTool - ?
* StateMod - ?

Additional information may need to be provided to explain how this StateMod dataset integrates with other CDSS models such as the StateCU consumptive use model.
Currently the focus is simply to demonstrate how the StateMod dataset can be maintained in GitHub while allowing data processing and StateMod runs.

## Using the Dataset ##

The following is a short guide on how to use the dataset:

1. Need to complete this as the repository is initialized.

## License ##

Currently there is no license for the dataset.  This topic is being discussed as CDSS software is moved to open source licensing.  The dataset is provided for public benefit to help with water resources planning.

## Contributing ##

CDSS is a program within the [Colorado Water Conservation Board (CWCB)](http://cwcb.state.co.us).  The primary contact for CDSS is [Andy Moore](mailto:andy.moore@state.co.us).

The Yampa dataset is maintained by [Wilson Water Group](http://www.wilsonwatergroup.com/) under contract with the State of Colorado and others.

## Release Notes ##

[2017-08-08] Initialize Git/GitHub repository using ym2015 dataset from CDSS website.