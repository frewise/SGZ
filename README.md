
#   What is it?
-----------------------
This repository contains the source code of the our publication [Sun, J. X., He, Y., Sanford, E., Montesion, M., Frampton, G. M., Vignot, S., ... & Lipson, D. (2018). A computational approach to distinguish somatic vs. germline origin of genomic alterations from deep sequencing of cancer specimens without a matched normal. PLoS computational biology, 14(2), e1005965.](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005965). The SGZ method is developed to allow researchers to distinguish somatic vs. germline alterations in cancer specimens without a matched normal in NGS data. 
  

#   Installation and how to run
  ------------------------
  FMI SGZ method does not require installation. The core method is implemented in python script fmiSGZ.py. Simply provide required files while calling the method in python terminals.
  
  After clone the repository or download and extract all files, run script 'run_test.py' to test if the scripts are working as expected. 'run_test.py' runs the basic SGZ method and FMI SGZ method on four test samples (provided). If the process succeeded, a message '-------Test succeeded.-------' should be printed on the standard output.

 
  
##   List of scripts and python module dependencies.

 All the scripts are developed under Python 2.7.6.
 
* `fmiSGZ.py`: the core SGZ method developed in Foundation Medicine Inc. to predict germline/somatic origins
* `basicSGZ.py`: a basic method to predict germline/somatic (inspired by *Jones, S., Anagnostou, V., Lytle, K., Parpart-Li, S., Nesselbush, M., Riley, D. R., ... & Galens, K. G. (2015). Personalized genomic analyses for cancer mutation discovery and interpretation. Science translational medicine, 7(283), 283ra53-283ra53.*)
* `run_test.py`: wrapper script to run both method on four test samples

The scripts were last tested successfully in python 2.7.14 with the following module dependencies:

* os
* sys
* glob
* argparse (version 1.1)
* logging (version 0.5.1.2)
* csv (version 1.0)
* scipy (version 0.19.1)
* numpy (version 1.13.3)
* filecmp


#   Contacts
  --------

  Please contact **Yuting He** <yhe@foundationmedicine.com> or **James Sun** <jsun@foundationmedicine.com> if you have any questions.
  
  Please cite the paper *Sun, J. X., He, Y., Sanford, E., Montesion, M., Frampton, G. M., Vignot, S., ... & Lipson, D. (2018). A computational approach to distinguish somatic vs. germline origin of genomic alterations from deep sequencing of cancer specimens without a matched normal. PLoS computational biology, 14(2), e1005965.* if you use SGZ in your publication.
