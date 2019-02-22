# Math Lectures

## What is in here

TODO

## Setting up a virtual environment

Set up a python virtual environment. 
(There are several ways to do this, my favorite is below)
Further reading on virtual environments in python can be found <a href="https://docs.python-guide.org/dev/virtualenvs/">here</a>, <a href="">here</a>, <a href="https://python-guide-cn.readthedocs.io/en/latest/dev/virtualenvs.html">here</a> and <a href="https://docs.python.org/3/tutorial/venv.html">here</a>.
</p>

```bash
virtualenv -p python3 .env
```

This sets up an entire python installation as an environment under the name `.env` which is not descriptive, but keeps me from having to remember how to activate all my different environments.

<p>
Next activate the environment, and install all the python dependencies via the requirements file. When the environment is active it will display to the left of the prompt, as shown below (where the $ symbol indicates your prompt.)
</p>

```bash
$ source .env/bin/activate
(.env) $ pip install -r requirements.txt
```

<p>
When finished with the repository or environment, you can deactivate it with the simple command deactivate.
</p>

```bash
(.env) $ deactivate
$ 
```

## Opening the Notebook

With your environment activated, you can run 

```shell
jupyter notebook
```

and it will launch in your browser. If not, it should give you a link to copy and paste into the browser. Then you can navigate any folders underneath the directory you ran your command and open the notebook.

Note that the notebook auto-saves, but you should still explicitly save it before exiting.

The notebook also suspends the interpreter between code blocks and keeps variables in scope much longer than you may be used to. If you have any weird issues, just restart and re-run the notebook.

## Troubleshooting

Problems with MatPlotLib on Mac OS are common and can have several different solutions. I am happy to help troubleshoot. 

For reference, [this](https://matplotlib.org/faq/osx_framework.html#osxframework-faq) talks about a few solutions in using `venv` vs. `virtualenv`.
