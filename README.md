# gp_creation

Step 1: create genome property DESC file from pathway csv file

reference files:
https://github.com/ebi-pf-team/genome-properties/blob/master/data/GenProp1433/DESC

https://www.ebi.ac.uk/interpro/genomeproperties/#GenProp1433

https://genome-properties.readthedocs.io/en/latest/flatfile.html#desc-file






Step 2: download the proteomes of the representative species of each pathway, and run interproscan on them.
Running Command: interproscan.sh -i input_file -d out_dir -f tsv -t p -pa -iprlookup
proteomes list: gp_test_proteome.csv





Step 3: merge all of the custom DESC files into a single file, and run the validate_GP.pl on it to validate the DESC file.





Step 4: after validation, merge it with genomeproperties.txt file and generate the csv file.

