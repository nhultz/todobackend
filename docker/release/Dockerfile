FROM nhultz/todobackend-base:latest
MAINTAINER Nick Hultz <nhultz328@gmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse