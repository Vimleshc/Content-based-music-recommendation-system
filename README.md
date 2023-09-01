# Content-based-music-recommendation-system
used Spotify dataset to give most similar songs based on songs content
The code first imports the necessary libraries, including pandas and sklearn.
Then, it reads the data from a CSV file and sorts it by track name. It then drops all duplicate track names, keeping only the first instance of each track.
Next, it defines a function called get_song_rec(), which takes a song name and a KNN model as input and returns the most similar songs to the input song. The function first creates a vector representation of the input song based on its energy, loudness, speechiness, acousticness, instrumentalness, valence, and tempo. It then uses the KNN model to find the k nearest neighbors of the input song. Finally, it returns the track names of the k nearest neighbors.
Finally, the code defines a main function that prompts the user to enter a song name and then calls the get_song_rec() function to get the most similar songs to the input song. It prints the track names of the k most similar songs.
