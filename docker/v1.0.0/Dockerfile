#---[2022/06/10 23:03] scafe:v0.9.0-beta as the base
FROM cchon/scafe:v0.9.0-beta

#---[2022/06/10 23:05] remove ./SCAFE dir
RUN cd .. \
&& rm -r /SCAFE/ \
&& git clone -v https://github.com/chung-lab/SCAFE 2>20220719190612 \
&& chmod 755 -R /SCAFE/scripts/ \
&& chmod 755 -R /SCAFE/resources/bin/ \
&& echo "export PATH=\$PATH:/SCAFE/scripts" >>~/.bashrc

#---[2022/07/19 19:06] change dir to start with
WORKDIR /SCAFE/

#---[2021/03/22 15:54] start bash when run
#CMD ["/bin/bash"]

