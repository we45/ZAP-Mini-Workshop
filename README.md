# OWASP ZAP 2.7.0 Mini Workshop

**This is still WIP. I should be done with the final version by 17 Jan 2018**

## Instructions

#### Requirements
* Download ZAP 2.7.0 from [here](https://github.com/zaproxy/zaproxy/wiki/Downloads)
* Python 3 (I am using Python 3.6.1)
* Docker

#### Install Instructions
* Clone the `git clone https://github.com/we45/ZAP-Mini-Workshop`
* I'd highly recommend using a `virtualenv` here
	* `cd ZAP-Mini-Workshop`
	* `virtualenv zap`
	* `source zap/bin/activate`
* Install requirements: `pip install -r requirements.txt` or `pip3 install -r requirements.txt` depending on how you are managing Python versions on your machine
* Start the IPython Notebook with `ipython notebook`. This should start the notebook and your default browser should automatically redirect you to the iPython Notebook
* Open the `ZAP 2.7.0 Mini Workshop.ipynb`, by clicking on it.
	* Install `Docker` if not already installed on your laptop. Pull image with this command: `docker pull abhaybhargav/vul_flask`
	* Run the Docker container with the command: `docker run -p 5050:5050 abhaybhargav/vul_flask`, you can add the `-d` optionally to run it as a detached process
* We'll go over the rest at the workshop :)