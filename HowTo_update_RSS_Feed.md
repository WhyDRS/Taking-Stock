## RSS feed tutorial 

- Bibic will compress files to Wix file limit of 50mb, and upload to the Wix backend. Bibic will add time length and filesize to the filename of each mp3 (this will be important later).
- Access RSS feed xml on Github and make an edit, or fork it depending on your level of access.
- Copy/paste previous episode at the top of the <item> list. (but below the main RSS feed info) Starting at <item>, ending at </item> 
- Change title of episode under <title>
- Change publish date under <pubDate>. This is the date the episode was recorded on X (typically 1 week after the previous episode). Format is Day of week (Mon/Tue/Wed/Thu etc), day of month (05/15/25 etc), month (Jan/Feb/Mar/Apr etc), year (2024/2025) and time (can be kept to 21:00:00 GMT regardless of actual timings)
- Replace mp3 url with latest episode from Wix backend in both url sections <enclosure url= and <guid isPermaLink="true">
- type="audio/mpeg" can be left as is
- Episode length (long number) enter the size of the mp3 in bytes (can be found by looking at the files properties on your computer, and will be at end of the filename on wix too)
- <itunes:duration> enter the length of the episode in hours, minutes and seconds. Round the second up or down depending on the decimal point in audacity.  If under an hour just write in minutes and seconds. No need to put 00 for hour. This should also be inluded on the filename.
- <author> can be left as is
- <category> can be left as is
- <description>: write in description after <![CDATA[<p>. Try to split it over 2 paragraphs (<p> </p>) as it looks  easier to digest on the phone apps.
- Twitter/X Link: add X link to space recording. Paste it both times, as this is hyperlink coding (once for the link and once for the text that is shown).
- Community links can be left as is
- Links and resources: each link needs a title above it. Links are currently displayed as the exact links they are for transparency. Be sure to put the link in as the hyperlink as well as the text. eg: <a href="https://www.youtube.com/@XXIMpod">https://www.youtube.com/@XXIMpod</a>
- Special thanks can be left as is
