# Assignment 1 part 1
## 1. Build Docker Image
* ```docker build -t docker-image-a1-p1 .```
* output : > 
[+] Building 10.8s (9/9) FINISHED                                                                                                                            docker:default
 => [internal] load build definition from Dockerfile                                                                                                                   0.1s
 => => transferring dockerfile: 199B                                                                                                                                   0.0s 
 => [internal] load .dockerignore                                                                                                                                      0.1s 
 => => transferring context: 2B                                                                                                                                        0.0s 
 => [internal] load metadata for docker.io/library/python:latest                                                                                                       0.0s
 => CACHED [1/4] FROM docker.io/library/python:latest                                                                                                                  0.0s 
 => [internal] load build context                                                                                                                                      0.1s 
 => => transferring context: 554B                                                                                                                                      0.0s 
 => [2/4] COPY app.py app.py                                                                                                                                           0.1s
 => [3/4] COPY requirements.txt requirements.txt                                                                                                                       0.1s
 => [4/4] RUN pip install -r requirements.txt                                                                                                                          9.9s 
 => exporting to image                                                                                                                                                 0.3s
 => => exporting layers                                                                                                                                                0.3s
 => => writing image sha256:2b91c9c8c0c32b132a53fa689621c0343ffe3ea86f6721d7c987fe3252a2f506                                                                           0.0s
 => => naming to docker.io/library/docker-image-a1-p1                                                                                                                  0.0s

* ```docker tag docker-image-a1-p1 saifullah3711/a_1_t_1```
* ```docker push saifullah3711/a_1_t_1 ```
* ```Using default tag: latest```
* The push refers to repository [docker.io/saifullah3711/a_1_t_1]
023800d05c10: Pushed
7f6fe586a0a5: Pushed
151e4a6a1981: Pushed
701d0b971f5f: Mounted from library/python
619584b251c8: Mounted from library/python
ac630c4fd960: Mounted from library/python
86e50e0709ee: Mounted from library/python
12b956927ba2: Mounted from library/python
266def75d28e: Mounted from library/python
29e49b59edda: Mounted from library/python
1777ac7d307b: Mounted from library/python
latest: digest: sha256:91cc552da0db85c7d791bb584e03b1bb5dc8cc693e7ad43a6e12e685e1629938 size: 2633

