# LearnOpenGL Starter Code

This repository is to help you get started with learning OpenGL. You can simply clone this repo and get started with the tutorial learnopengl.com without having to go through the hassle of setting up opengl extensions and glfw on your own

## Setup Instructions

* Fork the repo to create a copy of the repository on your own github account

![](https://i.imgur.com/lcwEAnE.png)


* Clone the repo
	```bash
	git clone --recursive https://github.com/{Your Username}/LearnOpenGL
	```
* The relevant opengl related header files are already included in ```main.hpp```. Instead of including ```<GLFW/glfw3.h>``` and ```<glad/glad.h>``` you only need to include ```main.hpp```

* You can build the project by running the following command in the root directory of the project
	```bash
	cmake -Bbuild -H.
	cmake --build build
	```
* You can run the project by running the following command in the root directory of the project
	```bash
	./build/Tutorial
	```
	OR
	```bash
	./build/Debug/Tutorial #(if your compiler is MSVC)
	```

* Try out the tutorial (try to write all the code on your own)