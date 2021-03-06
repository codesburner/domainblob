domainblob
==========
Domain Name Lookup Tool

Required Gems:
==============
* Nokogiri
* Whois
* Open-uri

How to use:
===========
1. Create a txt document named **totalPhraseList.txt** in the same directory as the script
2. When you run the script, with **ruby domainblob.rb** then it will use your root phrase to check over 5,000 potential domain names for availability.
3. When it is done, it will create a text document named after the phrase you used as your seed.
4. The script will process each line of the **totalPhraseList.txt** document, so put one seed word per each line and they will be run right after another.

How Long Does it Take?
=====================
It takes a while. We do not use the RegEx & Zone File method for finding domain name availability. While that would be fastest, I do not have Zone File Access and even if I did -- I would not be allowed to distribute that Zone File. So, instead we use 3 different methods to check if a domain name is available or not, and together these drive the domainblob domain name availability engine. Unfortunately, for the time being it takes more than 1 hour to check the 5,000+ possible domain names with the current system. I am looking into how we can make this faster moving forward, however -- that being said -- the reason we do the totalPhraseList.txt thing is so that you can line up a bunch of queries to be run right after another, and this way you can just keep the domainblob script running 24/7 if you would like.

License:
========
GNU GPLv3 (http://www.gnu.org/licenses/gpl.html)
