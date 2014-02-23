Open Public Library
=====================

The internet was presented to the public, we were promised that it would make 
all of the world's information available at the push of a button. For all the 
benefits it has brought us, it sadly fails at this goal. The vast majority of 
the world's creative works remain locked up by the entities that created them,
unaccessible to many. The Open Public Library seeks to change this, making the 
most important content freely available to any who seek it. 

This will be a digital library for the internet age.  The defining 
characteristic of this library will be that it focuses on sharing the best 
content freely with all who desire it.

In an effort to respect copyright, and not to seriously compete with the makers
of the works that will be in the library, no works will be accepted that are
less than five years old. This will also help the library to focus on more 
culturally relevant works, and not be overly swayed by every new trend that 
comes along.

The library itself will be driven by the works' meta-data, and all actual 
content of the works will be accessed over the internet through bit-torrent 
running on to of the TOR network. Unlike many websites that provide files over 
bit-torrent, the library will be curated as a coherent whole, not simply a 
collection of whatever files somone wishes to make available.

The whole of the content will be available online, but a "main collection" will
be split out.  This collection will be curated by the community, with the 
primary limitation being the total size of all the files in the main 
collection.

This limitation on size will be set by the size of commonly available storage 
devices. This will allow the main collection to be easily spread and shared, 
even where internet availability or bandwidth concerns would otherwise limit 
the library's availability. This will also insure its perpetual availability.

Current 16GB flash drives are generally available worldwide. This will be the
original size of the library. It will grow as readily available drives get 
larger.

Because of the size limitation, the content of the library will represent a 
balance between the importance of a work and its size. This way it would 
(initially) only have a few multi-gigabyte video files, but many sub megabyte 
text files. As the size of the main collection grows, there would be more space 
available for large video and audio files, but it would still be easier to 
include small text files.

Organization
---------------

The libraries content will be split into the following categories:

Text-Fiction (novels)
Text-Nonfiction (books, instruction manuals)
Text-Artistic (poetry, ???)
Text-Periodicals
Text-Encyclopedia (curated Wikipedia)
Video-Fiction (movies, tv shows)
Video-Nonfiction (documentaries)
Video-Artistic (music videos, nature time-lapses)
Audio-Fiction (radio plays, ??)
Audio-Nonfiction (podcasts, news reports, speeches)
Audio-Artistic (music)
Image-Artistic
Image-Historical

Within and across each of these categories, tagging will be used to define
subjects for all the works. Just as the works are curated by the community, 
the most important subjects will be curated by the community. These categories 
may be further refined to more closely match the categorization used by 
existing libraries.

Quality
---------------

There are currently many works available from various bit torrent sites. 
However, these are focused around providing the most recent content, not a 
library of the most important content. This causes various groups to compete 
with each other to be the first to release works to the public, instead of 
focusing on their quality.

The users of the Open Public Library will work together to provide the best 
possible quality of the works it curates. Works will not be made available to 
the general public if they determined to not be of sufficient quality. The 
users will submit different revisions of a work and the community will vote on 
and improve these works until one of sufficient quality is found. This will not 
be the end however, if an edition of better quality is created, the older copy 
will still be changed out for the newer copy. For text-based works, the 
differences between the current version and previous versions will also be 
kept.

Content Formatting Guidelines
These are simply initial suggestions, completely subject to community review.

Text
Works of text will be separated into works that are dependent on their layout, 
and works that can flow freely into different layouts (screen sizes, devices, 
etc.). All works will be formated in unicode. Works without flow dependencies 
will be kept in a common format such as doc book, html, or some type of 
database driven format. The library client will be used to convert this into 
formats for various e-readers. Translations of the text will also be available, 
these translations will use a find-replace like system with pairs of the 
original text and the translation.  Each translation will not be stored in a 
separate base format. For works that are flow dependent, they will be kept in 
the various native formats, but this type of work will be discouraged. 

In addition, text works may also be available in an audio-book format. In this 
case the audio book format will use the same format as the audio works. It will 
contain a file that converts timecodes within the audio to a location within 
the text. 

Video
Works of video will be stored as separate tracks for the video (with a high 
quality codec such as h.264, h.265, vp8, or vp9), audio (in various languages, 
stored in the same format as audio works), and subtitles (in various 
languages, stored as unicode text). The library client will convert this 
format into a single file to play on various devices. The video track of a 
work will be one of the following four options: sub 480p, 480p, 720p, and 
1080p all at 30 or 60 frames per second.

Audio
Works of audio will be stored in the FLAC lossless format (if more than 2 
channels, one FLAC stream per channel) and converted into various formats by 
the library client if desired. In addition to the actual audio, a transcript of 
the audio may be available. This transcript will be in the format for text 
works, but stored with the audio  (not to be confused with an audio book which 
is stored with the text, or audio/subtitles of video which are stored with the 
video).


Software
---------------
All content in the Open Public Library will be available for users to download
with nothing more than their web-browser, tor and a bit torrent client.  However, 
an additional client will be made available (and should be bundled with any 
content downloads). This will
allow users to convert content from the storage formats into various formats 
for reading, viewing, listening, etc. on various devices. It will also allow 
the user to *optionally* help with the curation process and distribution of the
content. 

In addition to allowing changes in format from those in the library, 
the client will allow the user to track all or part of the library and 
automatically download changes as they are made public.  It will also have the
feature of being able to import a (partial) copy of the library into the user's 
local copy of the library. For instance if a friend of a user attaches an 
external hard disk which contains part of the library to the user's computer, 
the user's version can be automatically brought up to date.

When the client installs, it will install a TOR client as well. It will also
setup as a TOR relay node and generate a hidden service for each install,
through which the user will accept bit-torrent connections. It will also ask 
the user if they wish to be a TOR exit node in addition to a relay node. Note
about TOR utilization: Generally TOR isn't good for bit torrent, but if all 
those installing the client are acting as relays for all the others who have
the client, this architecture shouldn't cause too much service degradation.

Curation Process
---------------
Users of the Open Public Library will be encouraged to assist in the curation
process by rating works both that are already in the library's Main Collection 
and works that have been submitted to the library but are not in the main
collection. Each work can be rated on a scale of 1-10 for both quality and
importance.

To ensure that people do not game the system, a web of trust will be setup to
verify a user's reputation amongst the community. Users can rate other users on 
a scale from 1-10 the same way they rate content. The reputation of this user
will weight their ratings of works.

To handle curation, there will be a central server, running as a TOR hidden
service. This will keep track of users and their reputation as well as ratings
of the various works. Each night, it will publish the history from the previous
day over bit-torrent so that all users of the client can see the latest ratings
of content and users.

On some schedule, to be determined, one of the library administrators would run 
an algorithm that would combine the quality and importance ratings with the 
ratings of the users that gave those ratings to determine overall ratings of 
the works. These would then be algorithmically selected based on their size to 
fit into the current size limitation of the Main Collection. Once this is
complete, a file representing the Main Collection would be published for all.

