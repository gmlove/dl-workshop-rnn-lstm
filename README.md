Tensorflow Environment Setup
============================

* Install docker-machine & virtualbox
    - brew install docker-machine
    - install virtualbox by click [here](http://download.virtualbox.org/virtualbox/5.1.8/VirtualBox-5.1.8-111374-OSX.dmg)

* Create virtual machine
    - docker-machine create -d virtualbox --virtualbox-memory 8196 tensorflow

* Look the ip of the virtual machine
    - docker-machine ip tensorflow

* Add this command into you environment file
    - eval $(docker-machine env tensorflow)

* Run the Docker container from the TW AI Club repository
    - docker run -p 8888:8888 --name tensorflow -v ${you-local-folder-of-this-repository}:/notebooks/ -d twaiclub/tensorflow-python3

* Go to: http://your-virtual-machine-ip:8888, and then you can do everything you want

* You also can use other ways to setup environment, just a reminder please provide as much memory as possible to match the computation need.

* If you can't make it to set up a local environment, you can use a pre-set-up environment at: http://10.17.4.181:8890/tree. Remember to create a folder by your name before you create any file.

* And there is a link about this course in [udacity](https://classroom.udacity.com/courses/ud730). You can get more information from it.
