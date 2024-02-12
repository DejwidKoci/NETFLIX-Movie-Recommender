# NETFLIX Movie Recommender

Welcome everyone visiting my GitHub!  
The aim of this project is to assign five productions to a selected film that are most similar in their characteristics.
To achieve this goal we use the `CountVectorizer` and `cosine_similarity` from the `sklearn` module. 

The database consists of 10000 productions with nine features (id, title, genre, original_language, overview, popularity, release_date, vote_average, vote_count). They come from a repository available on the [Kaggle](https://www.kaggle.com/datasets/ahsanaseer/top-rated-tmdb-movies-10k?resource=download).

In the `main.ipynb` file, a decision-making flow is presented in which the most similar films to the user's specified production are selected and the creation of files with the extension `.pkl` is performed, which are then used by the `app.py` file. 

In it, an application is in turn created using the `streamlit` framework, where the user selects the item of interest from a drop-down list of film productions. 

The output will be five productions with titles with assigned illustrations imported using the `request` framework from [themoviedb.org.](https://www.themoviedb.org/)

To run the application correctly, the `main.ipynb` file must be compiled. Then go to the python file `app.py` and compile it. In the terminal, type the following command:

```
streamlit run app.py
```

After this we will be redirected to the default browser with the running application.

The required python libraries are included in `requirements.txt`.
