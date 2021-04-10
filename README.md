# KGRulEm
Fact Checking via  Knowledge Graph Rules and Embeddings

### <a name="docker"> Running with Docker </a>

We've included a Docker setup for our tutorials to make setup easy.
First, make sure you have [Docker installed](https://docs.docker.com/install/) on your machine.
To build and run a Docker image for a tutorial, use `scripts/docker_launch.py` with the `--build` flag.

```bash
python3 scripts/docker_launch.py notebook --build
```

Building a Docker image from scratch can take anywhere between 5 and
30 minutes depending on the machine you're using.
We're working on making prebuilt images available via DockerHub.

Once the image has been built, a Jupyter notebook server will be available
on port 8888 (you can change the port with the `--port` command line option)
and print out a link you can follow to access the browser interface.
In your browser, open a `.ipynb` file you would like to run &mdash;
such as `01_spam_tutorial.ipynb` &mdash; and execute the cells in sequence.

Once you've built a tutorial-specific image for the first time,
you can run it without the `--build` flag:

```bash
python3 scripts/docker_launch.py notebook
```

