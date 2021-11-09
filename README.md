My Personal Site

Easier to develop in a docker container than having to maintain ruby versions:

docker run --rm -v ${PWD}:/srv/jekyll -p 4000:4000 -it jekyll/jekyll:4.0 /bin/bash bundle update && bundle install && bundle exec jekyll serve