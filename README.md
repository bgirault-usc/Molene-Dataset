This repository contains the original data of the Molène dataset that can be found on [data.gouv.fr](http://www.data.gouv.fr/fr/datasets/donnees-horaires-des-55-stations-terrestres-de-la-zone-large-molene-sur-un-mois/)

The original dataset, and this preprocessed dataset, are under the license [Licence Ouverte / Open Licence](https://www.etalab.gouv.fr/licence-ouverte-open-licence)

The original dataset is copied in the directory Original_Data, with the preprocessed CSV files.

The directory Matlab contains two versions of the datatset:
 - grasp_molene_data to use with the [GraSP](https://github.com/STAC-USC/GraSP) toolbox
 - gsp_molene_data to use with the [GSPbox](https://github.com/epfl-lts2/gspbox) toolbox

In both cases, the data is organized as a cell array of 3 graphs, each correponding to one kind of data (wind, temperature and rain). This maximizes the number of stations with complete data on the period, as not all reading are complete for all three kind. For each graph, the fields data_name and data contain two cell arrays of identical size respectively describing the exact data field and the data itself.

If you use this dataset in a scientific communication, kindly cite my [EUSIPCO 2015 paper](https://doi.org/10.1109/EUSIPCO.2015.7362637).