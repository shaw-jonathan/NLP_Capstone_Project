# Hidden Genres Using Clustering from Book Descriptions
The purpose of this project is to find correlations between books that go beyond their assigned genres. The written descriptions of the books will be the target of this analysis and modeling. 
## Data:
Data was taken by scraping a random assortment of books through OpenLibrary API.
https://openlibrary.org/dev/docs/api/books
Example book API - https://openlibrary.org/works/OL25312237W.json
10000 Books were scraped but only 2477 had actual descriptions that were used. 
## Model:
TFIDF Interpolation and K-Means clustering were utilized as unsupervised learning techniques. With the large quantity of description data, the optimal number of clusters was realistically between 100 and 150. 30 Clusters were chosen as compromise for the purposes of this project, but this sill presented good results.
## Plotting and Final Clusters:
Key features of each cluster were used to create unique labels and umap was used to visualize the data in 2D. Some of the resulting clusters were very interesting when compared to what the original genres of the books were.
