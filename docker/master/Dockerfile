FROM joshuawithey/base-multichain

COPY ./runchain.sh /root/runchain.sh
COPY ./blocknotify.sh /root/blocknotify.sh
RUN chmod a+x /root/runchain.sh
RUN chmod a+x /root/blocknotify.sh

ENV CHAINNAME=BiscitChain
ENV NETWORK_PORT=7557
ENV RPC_PORT=8002
ENV RPC_USER=user
ENV RPC_PASSWORD=password
ENV RPC_ALLOW_IP=0.0.0.0/0.0.0.0
ENV PARAM_TARGET_BLOCK_SIZE=target-block-time|30
ENV PARAM_ANYONE_CAN_CONNECT=anyone-can-connect|true
ENV PARAM_ANYONE_CAN_MINE=anyone-can-mine|true

EXPOSE 7557
EXPOSE 8002

CMD ["/bin/bash", "/root/runchain.sh"]