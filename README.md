# Docker for Data Science | Deep Learning

Ready-to-run Docker image containing Jupyter applications and interactive computing tools for Data Science and Deep Learning.

![docker logo](https://www.docker.com/sites/default/files/vertical.png "Docker")

## Specs
The image is built on top of python 3.6 (docker image) and has these packages built into it. It comes with the following installed packages:

  - Python Version: 3.6 
  - Tensorflow - 1.7
  - Tensorflow Object detection and its dependencies
  - Keras (latest)
  - Numpy 1.13.3
  - Scipy (latest)
  - Sklearn (latest)
  - Open CV (latest)
  - Scikit Image (latest)
  - Matplotlib (latest)
  - Seaborn (latest)
  - Jupyter Notebook (latest)
  - Pillow (latest)

The following ports have been exposed:
  - 8888 for Jupyter Notebook
  - 6006 for [Tensor Board]
  
[Tensor Board]: <https://www.tensorflow.org/guide/summaries_and_tensorboard>


It also comes with a collection of extensions that add functionality to the Jupyter notebook. For more information see [here].

## Setup

  1. Install Docker CE ([Install])
  2. Pull the image `docker pull achilleaskn/docker_data_science`

  3. Run the image (interactive mode) `docker run -i -t -p 8888:8888 achilleaskn/docker_data_science /bin/bash`

  4. Start Jupyter Notebook `jupyter notebook --port=8888 --no-browser --ip='0.0.0.0' --allow-root`

  5. Open your browser and go to localhost:8888 and use the password `thisismypassword` to login into the jupyter notebook


   
[Install]: <https://www.docker.com/community-edition>
[here]: <https://github.com/ipython-contrib/jupyter_contrib_nbextensions>
