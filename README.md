# cset-ml-for-polyglot-detection-artifacts
Artifacts for 2022 CSET Paper "Toward the Detection of Polyglot Files"
CSET URL: https://cset22.isi.edu/

The csv files containing the byte occurence vectors are arranged as follows:

name, label, path, [256 character vector where each index contains the number of times that hexadecimal value occured in the file]

The data is provided with (counts_train_magic_partial_X.csv) and without (counts_train_partial_X.csv) the mime type output of the file utility

The files with mime type (magic) contain an additional set of columns containing the possible mime types

These columns allow for one hot encoding of the mime type as an additional feature

The counts_train and counts_train_magic files were split into smaller files to evade github's 25mb filesize limit

Upon pulling the repo, use the command line to append the partial files back into a single file

We recommend loading the csv files into python using PANDAS, e.g., pandas.read_csv("FILE_NAME")

The models we evaluated were drawn from python packages SKLEARN and CATBOOST

