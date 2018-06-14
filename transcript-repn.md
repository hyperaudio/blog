When we first started working on Hyperaudio back in 2011, at the time [Interactive Transcripts](https://en.wikipedia.org/wiki/Interactive_transcripts) were relatively rare - that's when we started figure out how to represent timed-transcripts in a suitable manner, one that would work for both human and computer. I’ve been wanting to write this rather nerdy blogpost about that for some time.

In 2011 transcription services were few and far between, but one company that stood out from the crowd was [3Play Media](https://www.3playmedia.com/)- joyfully, submitting spoken-word audio to 3Play Media would result in not only the text representation but also structured data in the form of JSON. This JSON contained timings for each word transcribed, it's at that time we started thinking about how to represent and store Interactive Transcripts.

But let's back up a bit. What is an Interactive Transcript and why do they matter? There are various types of Interactive Transcript, we were interested in word-level timings, chiefly because we wanted to allow precise selection of words or phrases, so that people could, from the transcript, share and remix content.

Generally the advantages of including an Interactive Transcript with your media was to:

- Accessibility - as with captions or subtitles, including a transcript with your media makes it more accessible to those who cannot hear or properly understand the audio track.

- Navigability - an accessibility of sorts, which in our case means the ability to click on a word to move the associated point in the audio.

- Discoverablity - as long as you create your transcript statically on the server search engines will find it when crawling your page, making your audio or video more discoverable.

- Shareability - transcripts make it as easy to share the spoken word as it is the written word.

It's 2013 - I'm on the road from Providence, Rhode Island, my driver is Dan Schultz and we're headed to the MIT Media Conference in Cambridge, Massachusetts. Hyperaud.io has been funded by the Knight Foundation and we're starting to think seriously about what we're going to build. Together with Happyworm "partner-in-crime" Mark Panaghiston I'd been creating Hyperaudio-like applications for a couple of years now, through Mozilla I'd been lucky to work with media organisations as diverse as SoundCloud, Al Jazeera, WNYC and Danish Radio. We'd decided to represent Interactive Transcripts as HTML and have dubbed them Hypertranscripts. To take my mind off Dan's somewhat odd manner of driving (which involves periodically stepping on and off the gas to keep up speed) I decide to start a debate on how we should store transcripts.

Now I like HTML, it's relatively easy to parse for both human and machine and you can store it as a standalone file that can be rendered by any browser without any intermediary. Dan is, on the other hand firmly in the JSON camp, claiming it will be more flexible and easier to manipulate.








