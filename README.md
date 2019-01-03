README
project: Metadata - Torture - Visibility

About the Project

This project utilizes the API made available by the American Civil Liberties Union (ACLU) for their enormous resource for accessing US government documents related to the War on Terror, the ACLU Torture FOIA Database. The files here help you to grab the data from that system via API calls and save it locally for searching and utilizing in any way you like. 


Getting Started

You'll need to save the two python files into a directory of your choice and make a subdirectory in that same folder called "aclu_data". 


Running the Files

The Python scripts are listed here in order of application to achieve the final result:

    	aclu_api_get_data__.py
    	aclu_pull_docs_data_into_csv.py

There are just 2 python files. 
The first runs through all of the nodes on the ACLU's database to grab the full data for each record (documents and other record types). It saves each node's information as a separate JSON file.
The second python file goes through all of the JSONs and selects just the ones that represent government documents. It then grabs specific metadata elements and outputs them to a CSV file. This script can easily be modified to grab different metadata elements and/or work with JSONs that capture database data aside from document data.
The files are both annotated with more information on how to run them and what they do.


Notes

These scripts capture the metadata of the records in the database, which includes full OCR'd text and PDF file path. However, these scripts do not scrape the original PDFs of the documents. That functionality will be provided in a future update to this project via a separate file set.



**** THANKS!  ****  THANKS!  **** THANKS!  ****  THANKS!  ****

Thank you! To:
....
    Matt Miller  (for the excellent training and resources)
    Evan Volow (for sharing his example code for scraping government document repositories)
    Pratt Institute / Pratt School of Information

And ENORMOUS thanks to those who pushed for access to the orginal documents as well as provided scanned digital versions and their additional, extremely helpful metadata:
    American Civil Liberties Union (ACLU)
      and, in particular, Alexander Abdo formerly at the ACLU leading the Torture FOIA Database project and all the staff who worked on the project

Also thanks for help with earlier ideas related to this project are due to:
    New Media Lab (at the CUNY Graduate Center)
    CUNY Python Users Group (PUG)


