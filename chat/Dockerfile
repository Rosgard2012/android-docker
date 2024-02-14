FROM ekreative/android:33-ndk

RUN apt-get update \
&& ruby-install --latest \
&& ruby-install -i /usr/local/ ruby 2.7.1 -- --disable-install-doc \
&& gem update --system 3.1.6 --no-document \
&& gem install bundler:2.1.4 --force
CMD exec bash -l 

# RUN apt-get update \
# && rm -rf ruby-install-master && rm -rf ruby-install.tar.gz \
# && ruby-install --latest \
# && ruby-install -i /usr/local/ ruby 2.7.1 -- --disable-install-doc \
# && gem update --system --no-document \
# && gem install bundler:2.7.4 --force


#docker run --platform=linux/amd64 -it 0ddc2912c8d1 bash
#docker build --platform=linux/amd64 --tag rosgard2012/android-33-ndk:v04 -f Dockerfile .
##docker build --tag rosgard2012/android-33-ndk:v13 -f Dockerfile .
#docker system prune