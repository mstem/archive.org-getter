archive.org-getter
==================

Python script to download bulk results from Archive.org's TV News database of closed captions

Authors:
Rahul Bhargava and Matt Stempeck
MIT Center for Civic Media

TO USE THE SCRIPT:
Open the script in a text editor (like TextWrangler or BBEdit), edit line 11 of the code to change 'Your Query' to your preferred search term(s), and save it
Go to the command line (Terminal on a Mac, DOS or Cygwin in Windows)
Navigate to the folder that contains the script
Type in ruby archive.org-getter.rb and hit enter

Your results will show up in the same directory as the script itself. The results returned will be in JSON, the open data format. You can adjust how many results to return at once (by changing the ROWS variable in the script), but go easy on Archive.org’s servers: You’ll get your results faster (nearly instantly) in smaller batches of 200 or so.

Once you have your data, you can combine, clean, and parse it with Google Refine. I found ProPublica’s guide to cleaning messy data really helpful: http://www.propublica.org/nerds/item/using-google-refine-for-data-cleaning. You may also want to de-duplicate, because Archive.org records TV news broadcasts on the both the east and west coasts.

What you can do with it
Analyze a story: You could search for a specific story, like the recent controversial Steubenville rape case, and quickly get a sense of which news companies are covering the case and which words they use to talk about it. You can also share links to specific clips with your friends and colleagues.

You could also investigate our professional media’s treatment of a broader topic. You could trace the spread of the phrase “Obamacare” or watch the many breathless news segments covering “technology.”

Visualize TV news data: You’ll also have the data you need to visualize the lifespan of a story on televised news broadcasts. Archive.org renders a small line graph in your search results, but the JSON data will allow you to do much more.

For example, in the Trayvon Martin case study, we ended up normalizing the data with the number of Trayvon mentions in the printed press, blogosphere, on Twitter, and across other channels to determine when interest began and peaked.
