FROM ubuntu:18.04

WORKDIR /home/

COPY . .

RUN bash ./setup.sh

# Set the locale
RUN sed -i '/en_US.UTF-8/s/^# //g' /etc/locale.gen && \
    locale-gen
ENV LANG en_US.UTF-8  
ENV LANGUAGE en_US:en  
ENV LC_ALL en_US.UTF-8   

ENV PATH="/root/.cargo/bin:$PATH"
