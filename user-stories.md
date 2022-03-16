Data Registry User Stories

- As an end user in JupyterLab working with datasets.
    - When, I am working with datasets in a notebook
        - I would like JupyterLab to let me add them to “My Datasets”, so I can use them later
            - When, I am working with in memory datasets in a notebook (pandas, numpy, etc.)
                - I would like JupyterLab to be aware of those datasets, and let me add them to “My Datasets” using a UI, so I can use them later and see other things I might do with them.
                - I would also like to be able to quickly add them to “My Datasets” from Python explicitly.
            - When, I am working with remote data sources/sets in a notebook
                - I would to be able to quickly add them to “My Datasets” from Python.
            - When, I am working with in memory or remote datasets in a notebook
                - I would like to optionally see what else I could do with the data in other extensions
    - When, I am working with a dataset in another JupyterLab extension
        - I would like to see what else I could do with the dataset in other extensions and take action on that
        - I would like to be able to add the dataset to “My Datasets”
    - When, I am done using a dataset in “My Datasets”
        - I would like the dataset to be archived/deleted, so that it doesn’t appear in the list of “My Datasets“
    - When, I am working with a dataset in one JupyterLab extension and I want to use another JupyterLab extension to work with the dataset
        - I would like the extension to be able to access and work seamlessly with the dataset
        - I would like the extension to be able to carry the dataset changes from previous extension interactions
    - When I want to use an archived/deleted dataset again
        - I would like to see this dataset in list of “My Datasets”
    - When I want to find a dataset that I have already worked with
        - I would like to be able to search the dataset by name and other attributes/tags
    - When I am working with “My Datasets” in the data explorer
        - I would like to be notified when the dataset is updated (version changes)
- As a developer of a JupyterLab extension that inputs and/or outputs datasets (Notebooks)
    - When, I have an output dataset
        - I would like to show my user what else they could do with the output dataset in other JupyterLab extensions or notebooks and select one of those options in a simple UI, so I don’t have to build explicit integration with all of those extensions.
        - I would like to allow my user to choose to add the output dataset to “My Datasets”.
    - When I am building support for different types of input data
        - I would like to tell other extensions that I can do something with those types of data, so they can pass those types of data to me without my intervention and without me building explicit integration with all of those extensions.
    - When I am integrating with other extensions
        - I would like to interface with a central dataset API rather than all of the other extensions, so I don’t have to repeat the work of integration.
    - When a user imports a new dataset
        - I would like my extension to get notified, so that I can do something meaningful with the dataset, for example show in a list of “My Datasets”.
    - When another JupyterLab extension adds a new action for a dataset
        - I would like my extension get notified so that I can add a new option for the dataset so my end user can use this option perform the new action
    - When my user is done using the dataset
        - I would like my extension to be able to remove this dataset from “My Datasets”
    - When my end user wants to reuse an archived/deleted dataset
        - I would like my extension to be able to add this dataset to “My Datasets”
    - When a dataset is updated
        - I would like my extension to be notified, so that my extension can update the dataset info and user options related to this dataset
- As a developer of a data import experience in JupyterLab:
    - When a user picks a dataset they are interested in working with
        - I would like to show my user what else they could do with the output dataset in other JupyterLab extensions or notebooks and select one of those options in a simple UI, so I don’t have to build explicit integration with all of those extensions.
        - I would like to allow my user to choose to add the output dataset to “My Datasets”.




### Questions

- Do users want to add datasets to “My Datasets” by explicit action, or do they want extensions/notebooks to implicitly add datasets to “My Datasets”
    - Hypothesis: let users choose when to do this.

