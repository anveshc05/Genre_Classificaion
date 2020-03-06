## Genre Classification 

### Procedure
* **Song Selection** : Songs selected from [this database](https://github.com/indian-music-arch/IndianSongsDataset). Songs from all languages selected except the ones present in the normal folder to reduce the size and complexity of dataset due to a wide range of songs being present there.
* **Feature Extraction** : 
    * Features used ->
        * Spectral Centroid
        * Spectral Rolloff
        * Zero Crossing
        * MFCC
    * Clusters are generated and observed for each of the above mentioned features.
    * A combined feature vector of dimension 16x1 generated using the above mentioned features containing means and standard deviation of all the features. 2 data points are generated for the first 3 features. Top 5 MFCCs are obtained, mean and std for all the 5 are generated and appended to the combined feature vector
* **Clustering** :
    * Clusters are generated and observed for each of the above mentioned features.
    * Final results are generated for the case of 5 clusters generated on the combined feature vector as defined above.
* **Genre Identification** : 10-15 random songs present in each of the cluster are observed to identify a genre for the current cluster

### RESULTS

5 Genres observed : 
* Soulful
* Happy/Folk
* Energetic
* Classic
* Sad/Ambient