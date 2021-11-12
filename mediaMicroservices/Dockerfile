FROM thrift-microservice-deps:xenial

COPY ./ /media-microservices
RUN cd /media-microservices \
    && mkdir -p build \
    && cd build \
    && cmake .. \
    && make -j$(nproc) \
    && make install

WORKDIR /media-microservices
