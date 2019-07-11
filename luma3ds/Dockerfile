# until devkitpro/devkitarm is updated
FROM nanquitas/devkitarm

# install python3 + firmtool
RUN apt-get update && apt-get install -y python3-pip && \
	pip3 install git+https://github.com/TuxSH/firmtool.git

# build && install makerom
RUN cd home && \
	git clone https://github.com/profi200/Project_CTR.git && \
	cd Project_CTR/makerom && make && \
	mv ./makerom /opt/devkitpro/tools/bin/makerom && \
	rm -rfd Project_CTR
