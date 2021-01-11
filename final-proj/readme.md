# Final Project, Data Viz 2020
## Data 
The major part of the data was fetched from **Apple Music**. It is my main music service since mid-2019 There are such information as tracks I have been listening during the last one and a half year, duration of played tracks, how did I find them, etc. The secondary data source was **Spotify API** from which I was able to get detailed information almost for all tracks: album details, track danceability, valence, cover image.

## Motivation
The main goal was to get some insides about when and which music do I listen, find some periodical patterns meanwhile exploring new data visualization techniques (for example listening to Radiohead every autumn, Christmas songs every winter). It is a kind of self-reflection project. 

## Charts
### Artist 
[![Artist Chart](figs/artist-chart.png)](https://data-viz.vercel.app/artist-chart.html)

Interactive version https://data-viz.vercel.app/artist-chart.html


The idea was to show How my music preferences were changing during the last years and how many times every artist listened in a specific month.
The x-axis represents a timeline of my music history, the y-axis is the number of times I have listened to this artist in a specific month. 
Values are stakes in such a way that they represent the overall amount of music I have listened to during this month. Artists are sorted in such a way that the most listened located on the top of the stack. Color represents the specific artist. Separate dots appear in months when the certain artist is not represented in both the previous and next months. 
Not all artists represented on this chart, some "fleeting loves" were deleted to reduce visual chaos. 
The interactive chart helps to select specific artists using mouseover events or clicking on the legend above.
There are several insides which could be concluded:
- decrease in the amount of listened to music from the end of February till August. Possibly it is related to quarantine and there were not long trips to the office and back. Also, the interesting point that the music preferences changed after such a break (there are no connection between them) 
- a lot of bands continuously appear and disappear from my playlist and a lot of such return related to some personal experiences

### Album

[![Album Chart](figs/album-chart.png)](https://data-viz.vercel.app/album-chart.html)

Interactive version https://data-viz.vercel.app/album-chart.html
Here I want to visualize how old music does I like. There are album covers of artist I am listening located in such way that x-axis represents an album release date and y-axis represent a number of times songs from these albums have been listening. Also a cover image size increase with a number of listenings (double encoding which helps to distinguish a large number of albums at the bottom of the chart where). Y-axis is a log scaled which is not a good decision from a comparison point of view, but it also prevents extreme overlapping cause data are not smoothly located along axes. Albums were filtered with a threshold of 20 listenings. 
It is an interactive chart, mouse hovering a specific album the line will connect all artist covers and visually separate them from others. Such behavior made to introduce the ability to track the progress of individual bands.
My revelations:
- a lot of music I am listening to were created during the last decade
- there is a blank space in 70th, were there any good music except Pink Floyd?
- my favorite Radiohead album is The Bends (all my life I live with the idea it is In Rainbows)



### Genre
[![Genre Chart](figs/genre-chart.png)](https://data-viz.vercel.app/genre-chart.html)

Interactive version https://data-viz.vercel.app/genre-chart.html
These charts represent how  I discover new music and genres. There is a timeline on the x-axis. Every bar part represents a proportion of a certain genre in this month among newly discovered music. Tooltip provides additional information about the greatest discovery of this month - the most listened to song in this genre discovered in that month


Insides from this chart:
- Christmas songs every winter 
- electronic and techno since March 2020 related to visiting events.
- almost always alternative/rock music takes around 75% of my discovers 
- there are some mistakes and misleading in genre identifications in data
- April - July 2020, what Hip-Hop music is doing at the top of the chart? Quarantine time is definitely a strange one.

## Resources
- https://www.rcharlie.com/blog/fitter-happier


