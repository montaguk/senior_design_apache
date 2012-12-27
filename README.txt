in Ubuntu 12.04 the settings for apache2 are located in /etc/apache2. the
files contained in this repo can directly be copied to that location to set
up apache2 to communicate with django, although it won't really work or do
anything until the django file structure exists as defined in the other
repo.

notes: 
- the hosts file contained in this apache2 directory doesn't
  actually go in /etc/apache2, but should just be there as /etc/hosts. in
  order for the urls to work in django the hosts file has to be accordingly
  modified. it's possible that that file could simply be moved (mv) into /etc
  if that file has not been modified but I would do that with caution
