# The Running OWASP 2.8.0 Automation and Scripting Workshop

## Objective
I was really impressed by [Kelsey Hightower's](https://twitter.com/kelseyhightower)	"Learn Kubernetes the Hard Way". I really wanted to come up with something as simple and effective as that for one of my favorite DAST tools, [OWASP ZAP](https://github.com/zaproxy/zaproxy). Instead of making presentations that tend to be theoretical, rather boring and difficult to version manage and control, I decided to go the IPython Notebook route, where this could be an interactive experience and a running tutorial of sorts. 

This will be debuted as a 2 hour workshop at the proposed [OWASP Bay Area Meetup on the 24th of Jan 2018](https://www.meetup.com/Bay-Area-OWASP/)

The idea is to have a running interactive, totally hands-on, no-Death-by-Powerpoint :) training on OWASP ZAP Automation and Scripting. So, watch this space for updates :)

Please feel free to reach out for comments/requests on: 

- [Twitter](https://twitter.com/abhaybhargav)
- [LinkedIn](https://www.linkedin.com/in/abhaybhargav)
- [we45 LinkedIn](https://www.linkedin.com/company/1155059/)
- [Website](https://www.we45.com)

## Thanks
- I would like to thank the OWASP ZAP Development team led by [Simon Benetts](https://twitter.com/psiinon) for their great work with ZAP. It's probably the most powerful security tool for the Continuous Delivery Pipeline
- I would like to thank my own team at we45 for their work in integrating scanners and DevSecOps pipelines for our clients. 

## Instructions

#### Requirements
* Download ZAP 2.8.0 from [here](https://github.com/zaproxy/zaproxy/wiki/Downloads)
* Python 3.6.1
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

#### Update - 24 Jan 2018
* Added Automation for ZAP with Stored ZAP Sessions. 
* This can be accessed in the `ZAP Sessions` notebook
* Open the `ZAP Sessions.ipynb`, by clicking on it.

#### Update - December 12 2019
* Upgraded to OWASP ZAP v 2.8.0
* Tested Compatibility with Python 3
* Added `nbstripout` library for Output reduction