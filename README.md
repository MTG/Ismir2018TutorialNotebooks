# Ismir2018TutorialNotebooks

Jupyter notebooks for Ismir-2018 tutorial titled "Computational approaches for analysis of non-Western music traditions" by Serra, Clayton and Bozkurt. 
http://ismir2018.ircam.fr/pages/events-tutorial-09.html

To run a Jupyter server, we use docker.

## Install docker

### Windows
https://docs.docker.com/docker-for-windows/install/

### Mac
https://docs.docker.com/docker-for-mac/install/

### Ubuntu
https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/#install-docker-ce

## Run
In a terminal/console window, change to this directory

On MacOS or Windows, run:

    docker-compose up

On Linux, run the following (this command ensures that any files you create are owned by your own user):

    JUPYTER_USER_ID=$(id -u) docker-compose up

Then accesss http://localhost:8888 with your browser and when asked for a
password use the token created automatically and printed in the last line

Then, you can access the notebooks from the browser and run them.

## List of notebooks (ordered as presented in the tutorial):
* DownloadDataFromDunya_noToken.ipynb: demonstrates use of Dunya API to access CompMusic corpora
* downloadAllSARAGAContent.ipynb: notebook for downloading annotations, features, metadata and audio for the open access collections: Saraga-Hindustani, Saraga-Carnatic
* visualizeAnnotations.ipynb: visualizing manual annotations of Saraga dataset and performing some rhythm analysis tasks
* tuningAnalysis_SingleRecording.ipynb: case study for tuning analysis of a single recording in makam Huseyni
* tuningAnalysis_SetOfRecordings.ipynb: tuning analysis for a set of recordings from the same mode
* generateFileLists4Collections.ipynb: creating files-lists with mode information to help forming experiment subsets for mode recognition tasks
* formExpSubsets4ModeRecognition.ipynb: forms the subsets by grouping recordings with respect to mode or rhythm mode while also checking available files (ex: tonic annotation) for the recording
* symbolicDataPro_symbTr.ipynb: accessing pieces in a specific form and makam from the Turkish Makam Music Symbolic Data Collection (SymbTr), reading a specific a section of the form and ploting the melodic curves

The presentation files will also be shared soon within this repository.


