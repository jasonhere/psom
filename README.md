The pipeline system for Octave and Matlab (PSOM) is a lightweight library to manage complex multi-stage data processing. A pipeline is a collection of jobs, i.e. Matlab or Octave codes with a well identified set of options that are using files for inputs and outputs. To use PSOM, the only requirement is to generate a description of a pipeline in the form of a simple Matlab/Octave structure. PSOM offers the following services:
  * Run jobs in parallel using multiple CPUs or within a distributed computing environment.
  * Generate log files and keep track of the pipeline execution. These logs are detailed enough to fully reproduce the analysis.
  * Handle job failures : successful completion of jobs is checked and failed jobs can be restarted.
  * Handle updates of the pipeline : change options or add jobs and let PSOM figure out what to reprocess !

There is a [paper](http://www.frontiersin.org/neuroinformatics/10.3389/fninf.2012.00007/abstract) in Frontiers in Neuroinformatics that provides an overview of PSOM features and implementation. It is currently stable production stage and has been tested under Linux, Windows and Mac OSX (see the [page](https://github.com/SIMEXP/psom/wiki/PSOM-tests). To install PSOM, just download the latest [release](https://github.com/SIMEXP/psom/releases), extract the archive in a folder and add that folder to your matlab or octave search path. 
You're done ! You may have to adapt the [configuration](https://github.com/SIMEXP/psom/wiki/PSOM-configuration) to your local production environment. To use PSOM, you can have a look at the code of `psom_demo_pipeline`, or read [tutorial](https://github.com/SIMEXP/psom/wiki/How-to-use-PSOM).

PSOM is maintained by Pierre [Bellec](http://simexp-lab.org/brainwiki/doku.php?id=pierrebellec), "[Unité de Neuroimagerie Fonctionnelle](http://www.unf-montreal.ca/)" (UNF), "[Centre de Recherche de l'Institut de Gériatrie de Montréal](http://www.criugm.qc.ca/)" (CRIUGM), "[Département d'Informatique et de Recherche Opérationnelle](http://www.iro.umontreal.ca/)" (DIRO), [Université de Montréal](http://www.umontreal.ca/). 
The project was started by Pierre Bellec in the lab of [Alan Evans](http://www.bic.mni.mcgill.ca/~alan/) at the [McConnell Brain Imaging Center](http://www.bic.mni.mcgill.ca/), [Montreal Neurological Institute](http://www.mni.mcgill.ca/), [McGill University](http://www.mcgill.ca/), Canada. 
Core ideas have been inspired by the Poor Man's Pipeline (PMP) project developed by Jason Lerch, which was itself based on [RPPL](http://www.bic.mni.mcgill.ca/~jason/rppl/rppl.html) by Alberto Jimenez and Alex Zijdenbos.
