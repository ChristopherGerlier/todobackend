FROM gerlier/todobackend-base:latest
MAINTAINER Christopher Gerlier <gerlier@hotmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
  pip install --no-index -f /wheelhouse todobackend && \
  rm -rf /wheelhouse