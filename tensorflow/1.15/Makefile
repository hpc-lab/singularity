IMAGE=anaconda-2020.1-tensorflow-1.15.simg
ANACONDA_URL=https://repo.anaconda.com/archive/Anaconda3-2020.02-Linux-x86_64.sh

image: anaconda Singularity
	singularity build --fakeroot $(IMAGE) Singularity

anaconda:
	wget -q $(ANACONDA_URL)
	touch $@

all: image

clean:
	rm -rf $(IMAGE)
