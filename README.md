# eFiction customized for future combination with e107

IN DEVELOPMENT Still standalone efiction version but without conflicts with e107

This is just backup and notes...
THIS REPO contains files before changing efiction code itself. Main reason is for it is to have be able to start from beginning if integration ends badly. 


## Database changes 
*None*

Use the same prefix.

Prefix for e107: e107_
Prefix for efiction:  e107_ 

All efiction tables will look:
e107_fanfiction_xxx

All e107 tables will look:
e107_xxx

## Files

Only problem if you use e107 and efiction on the same level (what is the final goal):

index.php  
news.php
user.php
search.php
contact.php

### user.php
rename to member.php for efiction

Note: e107 clears sessions, so class2.php has to be loaded after get_session_vars.php  

### search.php

rename to searching.php for efiction

### news.php

removed

### index.php
e107 has to be used
- added recent menu to e107 menus

### contact.php

removed

Just notes: 

## Replaced functionality (it is already inbuilt in e107)

* Welcome message - delete from panels
* PHP info - delete from panels
* Custom pages - delete from panels

## Moved admin functionality 

* Custom pages (messages)  - efiction plugin, {FANFICTION_MESSAGES=message_name} for using in themes

