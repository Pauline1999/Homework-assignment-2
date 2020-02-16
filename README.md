# Homework-assignment-2
Computational musicology 

Since last week I had two inital ideas, I now decided to use this research question: 
How does the famous music style "Reggeaton" differ from German hip hop? 
Why is Reggeaton growing in popularity all around the world and German Hip Hop is not? Can we find a possible answer to this question?

Because after doing a lot of analyses I realized, it might be better to use playlists that include new but also old songs. The playlists I was going to use before included only the newest songs from each music style. I also decided not to use the playlists I created but rather use the most accurate ones I can find created by Spotify as this would exclude my subjective musical taste. Therefore, I do not project the tables and data from the analyses in this assignment but only the ones I created afterwards with the new playlists. 
The playlist I am using for the music style of Reggeaton is called "Reggeaton Classics" and includes 99 songs, which I think is very suitable. 
For the German Hip Hop I found a playlist by Spotify called "Deutschrap: Die Klassiker" but it only includes 50 songs. As I did not know if that is a problem I decided to create a new playlist including this and a second playlist by Spotify called "Modus Mio", and according to Spotify, it is the most important Hip-Hop playlists in Germany. I called this new playlist "German HipHop Classics". This playlist therefore ended with 100 songs. 

These are my tables for Reggeaton:

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

meanvalence | meanenergy | meanmode | meaninstrumentalness | meanliveness | meanloudness | meanspeechiness | meantempo | meandanceability | meanacousticness
-----|---|---|---|---|---|---|---|---|
   0.717  |    0.771   |   0.48     |       0.0108     |    0.180   |     -6.04       |   0.0992   |   109.     |       0.783 | 0.161
   
  sdvalence  sdenergy   sdmode    sdinstrumentalness  sdliveness    sdloudness  sdspeechiness    sdtempo sddanceability
   0.172     0.0909     0.502           0.0817           0.141         1.63         0.0613        30.7         0.0801
   
 meanacousticness
     0.161
     
 sdacousticness
     0.127    
     
 These are my tables for German HipHop: 
 
 meanvalence meanenergy meanmode meaninstrumentalness meanliveness meanloudness meanspeechiness meantempo meandanceability
  0.573      0.666       0.34           0.00804        0.173        -6.81           0.209        111.            0.737
  
 sdvalence   sdenergy   sdmode    sdinstrumentalness   sdliveness   sdloudness   sdspeechiness   sdtempo   sddanceability
   0.213      0.119     0.476             0.0417        0.102         1.95          0.132         30.0           0.103
 
 meanacousticness
     0.187
     
 sdacousticness
     0.163
   
 As I just created these new playlists the results I got from those tables are different from the results I had in my first analyses. 
The differences I can find from these tables are a little less satisfying than the results I had at first therefore, I will tried to enrich my data with more visualizations. From these visualisations I can see and interpret diffences much more easily. 

I missed last weeks class and I do not know how to insert the visualisations on Github as there is some error when trying to commit changes via R studio. I can therefore not provide the images in this assignment but online give some descriptions.  

As I experience Reggeaton as very positive and moving, in terms of danceable, music I for instance created a ggplot with valence on the x axis and danceability on the y axis. 

ggplot(playlist_audio_features, aes(x=valence, y=danceability)) + geom_point()

The songs for German Hip Hop were distributed much more central than the Reggeaton songs. I expect this to also be one of the reasons for its popularity all around the world. 

Additionally, because I perceive both Reggeaton and German Hip Hop as very loud and fast I created a ggplot with the loudness and tempo of the songs. 

ggplot(playlist_audio_features, aes(x=loudness, y=tempo)) + geom_point()

The plots showed a similar shape of distribution but the Reggeaton songs  were noticeably a lot distributed for a tempo of circa 95. Because Reggeaton has this specific beat that occurs in almost all songs I think it will be very interesting to look deeper into this. 

Through my new analyses I thought more about why I myself like Reggeaton and what I perceive to be specific features of it. This gave me ideas for visualisations and I think I will be able to find interesting results when comparing Reggeaton to German Hip Hop. 

