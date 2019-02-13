# Setup

To setup local environment, we use Docker to ease things out. If you don't have Docker yet please install
* [mac](https://docs.docker.com/docker-for-mac/install/)
* [windows](https://docs.docker.com/docker-for-windows/install/)

Then clone this repository
```sh
git clone https://github.com/tw-th-data-guild/essential-data-developer.git
```

After that, we can run this in the root repository
```sh
docker run -p 8888:8888 -v "$PWD":/home/jovyan jupyter/datascience-notebook
```

And you will see something like this
```
Executing the command: jupyter notebook
[I 10:21:54.144 NotebookApp] Writing notebook server cookie secret to
/home/jovyan/.local/share/jupyter/runtime/notebook_cookie_secret
[I 10:21:54.755 NotebookApp] JupyterLab extension loaded from
/opt/conda/lib/python3.6/site-packages/jupyterlab
[I 10:21:54.755 NotebookApp] JupyterLab application directory is
/opt/conda/share/jupyter/lab
[I 10:21:54.758 NotebookApp] Serving notebooks from local directory:
/home/jovyan
[I 10:21:54.758 NotebookApp] The Jupyter Notebook is running at:
[I 10:21:54.758 NotebookApp] http://(e6ee7e1fcd25 or
127.0.0.1):8888/?token=58b03f3ad9152656beaeb12af664e440c4c180cf4b2413bd
[I 10:21:54.758 NotebookApp] Use Control-C to stop this server and shut down all
kernels (twice to skip confirmation).
[C 10:21:54.760 NotebookApp]
    Copy/paste this URL into your browser when you connect for the first time,
        to login with a token:
                http://(e6ee7e1fcd25 or 127.0.0.1):8888/?token=58b03f3ad9152656beaeb12af664e440c4c180cf4b2413bd
```

Open your web browser of choice and go to `localhost:8888/?token=your-token`.

Try out `week1/iris.ipynb` and run all the cells (`Cmd + Shift + p` or `Ctrl + Shift + p` and type run all cells).
If you see no error then it should be good.
