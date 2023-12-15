# youtube-data-harvesting-and-warehousing
  details of youtube channels are extracted they are uploaded to MongoDB and shifted to SQL as table and imported to streamlit
  
REQUIREMENTS
#packages needed to be installed
  1.pymongo
  2.psycopg2
  3.pandas
  4.streamlit
  5.google-api-python-client
#Getting API of youtube
#API stands for Application Programming Interface
#API of youtube has been extracted from google cloud console
#Sign in to mongoDB
#Install postgres 

#Process
step 1 : importing packages (line 1-5)
step 2 : connection is given using API(line 7-15) 
step 3 : getting channel details using channel ID from youtube (line 17-35)
step 4 : getting playlist IDs of required youtube channel(line 40-65)
step 5 : getting video IDs of required youtube channel(line 68-89)
step 6 : getting video details such as title,published date & time,likes,dislike,comments,etc for required youtube channels 
         by using video ID extracted above(line 92-120)
step 7 : getting comment details for particular video from extracted video ID(line 124-148)
step 8 : connection to mongoDB(line 153-154)
step 9 : uploading extracted details like channel details,playlist information,video information,
         comment information to mongoDB(line 158-169)
step 10 : connection to postgres(line 173-178)
step 11 : creation of channel table in postgres with channel information(line 172-229)
step 12 : creation of playlist table in postgres with playlist information(line 232-287)
step 13 : creation of video table in postgres with video details(line 290-378)
step 14 : creation of comments table in postgres with comment details(line 381-435)
step 15 : assigned under one function(line 438-443)
step 16 : creation of streamlit page with necessary details (line 487-632)

  
  

  
