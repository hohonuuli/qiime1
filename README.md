# qiime1

[Docker](https://www.docker.com/) container with [Anaconda](https://www.continuum.io/), [qiime](http://qiime.org/), [R](https://www.r-project.org/), [Java](http://openjdk.java.net/), [RDP Classifier](https://github.com/rdpstaff/classifier), [ChimeraSlayer](http://microbiomeutil.sourceforge.net/), [Mothur](https://www.mothur.org/), [Muscle](http://www.mybiosoftware.com/muscle-3-8-31-multiple-sequence-alignment.html), [rtax](http://qiime.org/tutorials/rtax.html), and [Swarm](https://github.com/torognes/swarm).

It's a beast of a Docker container.

## Usage

To start an interactive session, first start a bash shell into the container.

```
docker pull mbari/qiime1
docker run --name qiime1 -v /Path/to/data:/mnt/data -i -t mbari/qiime1 /bash/bin
```

Once inside the container you just need to run:

```
source activate qiime1

# Your data will be in /mnt/data if you used the docker run command above
```