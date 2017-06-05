# Multicentric_glioma_CN
Copy number scripts for multicentric glioma study

#Setup (once)
Run Rscript 0.setup.R once. 
This will setup links to shared annotation data sets and lab data files on the TIPCC compute cluster.
Make sure ./config.yml is correct. It specifies the default analysis settings. 

The individual entries can be overridden by individual command-line options to the Rscript calls.


#Data processing
#The following scripts should be run in order:

Rscript 1.mpileup.R
Rscript 2.sequenza.R
Rscript 3.pscbs.R
Rscript 4.reports.R

You may adjust ./config.yml when new files come in, or you can override the defaults individually via command-line options.
