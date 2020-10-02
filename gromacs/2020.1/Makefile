IMAGE=openmpi-3.1.6-gmx-2020.1.simg
OPENMPI_URL=https://download.open-mpi.org/release/open-mpi/v3.1/openmpi-3.1.6.tar.bz2
GROMACS_URL=http://ftp.gromacs.org/pub/gromacs/gromacs-2020.1.tar.gz

image: Singularity openmpi gromacs
	singularity build --fakeroot $(IMAGE) Singularity

openmpi:
	wget -q $(OPENMPI_URL)
	touch $@

gromacs:
	wget -q $(GROMACS_URL) 
	touch $@

clean:
	rm -rf $(IMAGE)
