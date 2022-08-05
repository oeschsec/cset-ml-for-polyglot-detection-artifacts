# cset-ml-for-polyglot-detection-artifacts
Artifacts for 2022 CSET Paper on Polyglot Detection Using Machine Learning

the csv files containing the byte occurence vectors are arranged as follows:
name, label, path, [256 character vector where each index contains the number of times that hexadecimal value occured in the file[

the data is provided with (counts_train_magic_partial_X.csv) and without (counts_train_partial_X.csv) the mime type output of the file utility

the counts_train and counts_train_magic files were split into smaller files to evade github's 25mb filesize limit

upon pulling the repo use the command line to append the partial files back into a single file

