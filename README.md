# gogetit
Torrent RSS downloader with streaming capability

This is my first attempt at creating a program outside of bash. 
It's intended to catch an rss feed's data at a specified interval, parse for matches to keyword, and download the first match only. 
We expect this to be a series, hence a start sequence ex [s02e05] which increments after finding a match to either the next episode in same season, else first episode of next season.
Accepted client will be using transmission, with the RPC API in order to add the torrent. 

First version is more a proof of concept with no UI, or streaming capacity.

The next goal is to create a UI which requires auth to view, and has capacities off the top of my head:

- list file and associated torrents which have been successfully downloaded
- delete unsatisfactory file/torrent (causing a research)
- download the file
- stream the file directly in browser
- obtain program/show information from external API

There should be no reason why this app can't be installed on a remote VPS the same as a home computer. I'm uncertain if this will all be possilbe with Go libraries or if I will need to use javascript libraries for some functionality. 
Overall I want something sufficiently challenging that I can chew on over time, and not get burnt. This doesn't appear to be too ambitious for a first project. 
I will advise anyone who wants to try this app in production to first look over the source code, and test. I can't state clearly enough that this is my first attempt at programming in any language outside of bash. 

*You use this at your own risk!*
