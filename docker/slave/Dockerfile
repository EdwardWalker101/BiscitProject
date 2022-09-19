FROM joshuawithey/base-multichain

ADD ./runchain.sh /root/runchain.sh
RUN chmod a+x /root/runchain.sh

ENV CHAINNAME=BiscitChain
ENV NETWORK_PORT=7557
ENV RPC_PORT=8002
ENV RPC_USER=user
ENV RPC_PASSWORD=password
ENV RPC_ALLOW_IP=0.0.0.0/0.0.0.0

EXPOSE 7557
EXPOSE 8002

CMD ["/bin/bash", "/root/runchain.sh"]
