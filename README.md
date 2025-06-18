# TFM

## Note: The full Dataset is available on Zenodo: https://zenodo.org/records/15687654
This repository is part of my Master's thesis for the Master's in Computational Social Sciences at Universidad Carlos III de Madrid.

This repository holds the code and materials for a text analysis project. It explores gender representation in popular music lyrics. The project uses the "Spotify 12M Songs Dataset" from Kaggle, which gives metadata and audio features for many songs. For better analysis, the original dataset received more information. We added artist gender, country of origin, genre, and popularity using public APIs like MusicBrainz and Spotify.

The workflow uses four Jupyter notebooks:

The first notebook (01_data_collection.ipynb) loads the original dataset. It then adds metadata by sending REST API requests. Artist profiles get gender and origin details. We also pull popularity and genre information from Spotify. Lyrics are gathered through spaced API queries because there are limits on requests.

The second notebook (Data_analysis.ipynb) merges all the data parts into a single comprehensive dataset, since lyrics and metadata had to be retrieved in multiple batches due to file size constraints. A brief initial exploration of the dataset is also included.

The third notebook (main_spanishlyrics.ipynb) performs the main text analysis for Spanish lyrics. Gender-related keywords are identified, and context words surrounding them are extracted, counted, and visualized to understand how men and women are described in Spanish-language music.

The fourth notebook (main_englishlyrics.ipynb) applies the same methodology to English lyrics, allowing for cross-linguistic comparisons in the representation of gender across songs.

The final dataset includes detailed audio features, artist metadata, and preprocessed lyrics, and forms the basis for the subsequent linguistic analysis. This work aims to shed light on common patterns and associations related to gender in both Spanish and English music texts.
