FROM zblizzard/todobackend-base:latest
MAINTAINER Zach Blizzard <zachary.blizzard@gmail.com>

# Copy application artifactcs
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
	pip install --no-index -f /wheelhouse todobackend && \
	rm -rf /wheelhouse
