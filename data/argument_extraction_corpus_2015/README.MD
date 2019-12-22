Argument Extraction Corpus
 
StartComplete
Thank you for your interest in our work. Below you will find links for various files.

Corpus
Download the SQL database (25.7Mb, compressed).

This is the SQL database that stores all the data used in these experiments. It includes ~109,000 posts on the topics of gun control, gay marriage, evolution, and the death penalty. Because it is partially built from the Internet Argument Corpus, please cite both of the following papers if you use this in your reserach:

Argument Mining: Extracting Arguments from Online Dialogue. Reid Swanson, Brian Ecker, Marilyn Walker. In the 15th Annual SIGdial Meeting on Discourse and Dialogue, Prague, CZ

A Corpus for Research on Deliberation and Debate. Marilyn A. Walker, Pranav Anand, Jean E. Fox Tree, Rob Abbott, Joseph King. LREC 2012

### Setup:

Decompress with xz -d iac_for_sigdial_2015_v1.sql.xz

Setup the schema in mysql with the command: CREATE SCHEMA schema_name DEFAULT CHARACTER SET utf8mb4 DEFAULT COLLATE utf8mb4_bin;

Then import to that schema: mysql -u root -p schema_name < iac_for_sigdial_2015_v1.sql

## Annotated Data
Download the annotated training and testing data for each topic (348 Kb zipped)

These are the (processed) mechanical turk annotation results. They contain a phrase per row, and an annotated score. The "GoodSliderMean" column gives the mean annotated score after some annotations have been dropped do to poor reliability. "GoodSliderDev" is the standard deviation. "Connective.x" lists whether or not one of our selected connectives is included in the phrase. "ResponseInitial.x" lists whether or not the connective begins the phrase. ItemId is a hash that can be used as a unique identifier.

Please cite the following if you use these in your work:

Argument Mining: Extracting Arguments from Online Dialogue. Reid Swanson, Brian Ecker, Marilyn Walker. In the 15th Annual SIGdial Meeting on Discourse and Dialogue, Prague, CZ

https://nlds.soe.ucsc.edu/node/29/done?sid=7036&token=8d28be8515f700b323ef7da5f7ff97e6