download_and_build: downloaded all

DATAFILE=data.tgz
RVIZ_DATAFILE=UWSim-dta-rviz.tgz
LEARNING_DATA=learningData.tgz

downloaded:
	wget http://www.irs.uji.es/uwsim/files/$(DATAFILE) && tar xvf $(DATAFILE) && rm $(DATAFILE)
	wget https://sites.google.com/a/uji.es/learning/install/$(LEARNING_DATA) && tar xvf $(LEARNING_DATA) && rm $(LEARNING_DATA)
	touch downloaded

rviz-data:
	wget http://uji-ros-pkg.googlecode.com/files/$(RVIZ_DATAFILE) && tar xvf $(RVIZ_DATAFILE) && rm $(RVIZ_DATAFILE)

include $(shell rospack find mk)/cmake.mk

