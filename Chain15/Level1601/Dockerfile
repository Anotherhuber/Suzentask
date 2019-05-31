FROM bash

ARG FLAG

RUN adduser -D suzen 

ADD hello /bin/hello

USER suzen
WORKDIR /home/suzen

RUN mkdir -p /home/suzen/garden/tree && mkdir -p /home/suzen/stone/litle stone/ &&\
mkdir -p /home/suzen/grass/cave

ADD .chest /home/suzen/garden
ADD NISHA /home/suzen
ADD .hidden /home/suzen/garden/tree
ADD PijamaLama /home/suzen/grass/cave

RUN sed -i "s/FLAG HERE/${FLAG}/g" /home/suzen/garden/.chest





ENTRYPOINT ["/bin/hello"]

