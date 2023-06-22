# Introduction
  Music preference is a universal phenomenon that reflects people’s personality, culture, and environment. People listen to music for various reasons such as entertainment, relaxation, emotional regulation, socialization, and cultural identity expression. Music preferences vary across individuals and societies, and are influenced by various factors such as age, gender, education, socioeconomic status, and media exposure. In recent years, researchers have paid increasing attention to the relationship between music preference and cross-genre music consumption, which refers to the tendency to listen to music of different genres. Understanding this relationship is important because it can shed light on the mechanisms of music preference formation and the potential benefits of cross-genre music exposure. In this study, we investigate the relationships between preference for music of different genres and tendency to listen to music of other genres, using Croatia, Hungary, and Romania as examples. These countries have distinctive music cultures and histories and provide an interesting context to explore the diversity and commonality of music preferences and behaviors.

  The topic is relevant as music preference is a universal phenomenon that is closely related to the individual's personality, social and cultural background, and emotional responses. Additionally, the tendency to listen to music of other genres may reflect an individual's openness to different experiences and cultural backgrounds. Therefore, investigating the relationship between music preference and the tendency to listen to music of other genres can provide insights into the cultural and psychological aspects of music consumption in different societies. 

  Talking about novelty while there are some studies on the relation between music preference and music listening behaviour in certain regions, there is little research on comparing the three countries, Croatia, Hungary, and Romania, which belong to similar cultural and historical backgrounds but have their own unique cultural heritages and contemporary music scenes.
Research question: What is the relationship between preference for music of different genres and the tendency to listen to music of other genres in Croatia, Hungary, and Romania? Are there any cross-cultural differences in this relationship? 

### Hypothesis 1: 
People who listen to pop music tend to be more interested in a variety of music consumption and listening to all other genres as well.

### Goal:
To examine international trends in preferences for music of different genres and to determine the relationship between love for one genre and tendency to listen to music of other genres, using three countries as examples.

# Objectives:
1. To collect data about what kind of music genres people in three countries (Croatia, Hungary and Romania) prefer.
Using statistical methods, estimate people's tendency to listen to other genres of music, if any.
2. analyze the data to come up with an overall picture of international music preference and the relationship between music genres in the three countries.
3. Draw conclusions about the relationship between musical genres and propensity to listen to them across cultures and countries, as well as the general international trend in musical tastes.



# Metodology
## Data
Data is taken from [Stanford Large Network Dataset Collection](https://snap.stanford.edu/data/gemsec-Deezer.html). The data was collected from the music streaming service Deezer (November 2017). The csv files contain the edges -- nodes are indexed from 0. The json files contain the genre preferences of users -- each key is a user id, the genres loved are given as lists. Genre notations are consistent across users. In each dataset users could like 84 distinct genres. Liked genre lists were compiled based on the liked song lists. The countries included are Romania, Croatia and Hungary. 

## Methods   
  The original plan formed before to analyze users was defeated by large datasets with more than 50k years each and more than 1 million connections. Therefore genre preference analysis was chosen. First of all csv tables were generated from genre.json tables, by creating a matrix showing how many users listen both of the chosen genres (for ex:  HR_relations_heatmap.csv). Then the heatmaps were constructed.

  In the application can be finded the code we created to show heatmaps (See Appendix 1-3). Heatmaps is a generic term that embodies a kind of graphical representation of data. In our case, the dataset consists of users and their music preferences on a Dezeer. It must be mentioned that we state the threshold of 2000 listeners for showing genre in heatmap, it is made for better vusialusation because of big number of possible genres.

  We processed the data and made all sorts of combinations - how many people of one style listen to some other style (for example, how many metal fans also listen to pop music). Then we divided these numbers by the total number of listeners of one of the genres to get relative values. That is, the numbers in the cells are *fractions* of the total values. 

  In this task, we are dealing with a pairing where a person has two preferences. Therefore, we considered that in all genre pairs, the number of fans of each genre is different. To answer the question of how many people among Indie rock fans are also fans of Alternative rock, we need to look for a column of Indie and a row of Alternative rock (Appendix 5).
Otherwise, if we want to understand how many fans of Alternative are also into Indie, we look for the column with Alternative and the row with Indie.
The values in the cells are fractional, rounded to 1 decimal place. They can be regarded as a percentage (for example, 0.7 = 70%). In this case, a value of 0.5 is sort of an average correlation, 1 is a strong correlation, less than 0.5 there is no correlation.
A similar analysis of musical genre correlations was conducted for all three countries under consideration.

## Analysis
### Romania
  If we talk about the reciprocal preferences in music among Romanian listeners, the following key trends can be highlighted. Indie listeners have representatives of almost all other musical genres in their playlists. Thus, Indie listeners have a willingness to listen to other music genres in all their diversity and quite often. But the least interest in any other genres of music, except for one key genre, tends to be the lovers of rugby, classical music, latino music, hard and indie rock. There are also exceptions, for example, people who listen to metal also often happen to listen to hard rock. Nevertheless, the most diverse in musical consumption among the Romanian population are those who listen to pop music and light rock. That is, the main trend for this country is the fact that most people like only similar/similar sounding music, with the exception of pop music fans.

### Croatia
  If we turn to the temperature map of Croatia and look at which music lovers also willingly listen to other genres, in this country the number of people fans of different music genres is observed among more genre lovers. As in the case of Romania Croatia the main diversified listeners are also not fans of pop music, while a high correlation is observed among fans of indie similar to the previous example. But in the case of Croatia, the category of people who listen in addition to one favorite musical genre tends to like other music, also included fans of dance music, most indicators are close to one for all other music genres. Also among users from Croatia and fans of alternative music there is a love for Indian rock, disco music, hard rock, electro, reggae, which also indicates a relative openness to other genres. 
But fans of genres such as blues, Latin music, indie-pop, jazz, and classical music remain mostly committed to one particular genre of music. What, in fact, we also observed in Romania for the fans of these genres.

### Hungary
Speaking of the results of the heat map of Hungary we can also trace the familiar tendency that fans of pop music are not open to listening to other music genres as others as well. Interestingly, in Croatia, together with fans of pop music, fans of dance music, electro, rock and, in some cases, alternative music are the most open to listening to other music genres. Note that in none of the previous countries representatives of alternative music were not ready to listen to love other musical genres. If we talk about the opposite, the lowest correlation observed fans of jazz, reggae and East Coast music, the figures in this case is very close to zero and demonstrates the willingness of fans of these genres to listen to any other music.

## Conclusion
Based on the trends observed in the three countries, it can be concluded that there is interesting that the most listenable genre fans of pop, are not to be more open to exploring other music genres. This fact reject th hypothesis. However, fans of other genres, such as indie, rock and classical music, tend to be more committed to their preferred genre. The findings also suggest that there are some similarities in musical preferences across the three countries, with Indie music being a common favorite among listeners and the Pop is most listenable. However, there are also differences in the openness of fans of different genres to explore other genres, with some countries showing more diversity in musical consumption than others. Overall, the trends suggest that there is a diversity in musical tastes among the population of these countries, but there are also strong clusters of listeners with similar tastes.

# APPENDIX.
### Appendix 1. Heatmap Romania.
![Quantity Romania](https://github.com/Booglik/Course-SNA-project/assets/72690848/142778e4-21a2-4afd-a4c2-403e1eca76ec)
![Heatmap Romania](https://github.com/Booglik/Course-SNA-project/assets/72690848/3b0a1f5f-9c00-40ad-9429-b161d822991c)

### Appendix 2. Heatmap Croatia.
![Quantity Croatia](https://github.com/Booglik/Course-SNA-project/assets/72690848/1b47188d-4f95-4099-b65d-65022f610eed)
![Heatmap Croatia](https://github.com/Booglik/Course-SNA-project/assets/72690848/8041a3de-b4c8-463b-b1f0-26145820fa38)

### Appendix 3. Heatmap Hungary.
![Quantity Hungary](https://github.com/Booglik/Course-SNA-project/assets/72690848/8c1b307d-0490-4b09-8492-4b0d2b4a86ae)
![Heatmap Hungary](https://github.com/Booglik/Course-SNA-project/assets/72690848/55eca7b2-e18c-4726-bd7d-420f0f9d99c8)

### Apendix 4. Top genres within the countries
![subplots](https://github.com/Booglik/Course-SNA-project/assets/72690848/c4c82d51-3dbe-45af-bb78-8629c776aaa8)

### Apendix 5. ![How to use](https://github.com/Booglik/Course-SNA-project/assets/72690848/53605a81-7edd-4418-a660-92f15b1530f9)
