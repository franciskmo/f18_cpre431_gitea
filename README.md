# f18_cpre431_gitea
Explanantion of Gitea v1.4.0 exploit.

Based on the work of Kacper Szurek, [who found the exploit.](https://security.szurek.pl/gitea-1-4-0-unauthenticated-rce.html)

This repo includes a modified version of the script written by Kacper, the necessary session file, and a sample bash script.

To set up you'll need to have the following installed:
* Python 2.7
* Pip
* Virtualenv

To create a virutal environment:`virtualenv venv`

Activate with: `source venv/bin/activate`

Exit Venv with `deactivate`

Install the python dependencies:
`pip install -r requirements.txt`

To run:
`python2.7 exploit.py <Address of gitea server> <Path to sh script>`

For example to run on a local gitea server with our provided bash script:
`python2.7 exploit.py http://localhost:3000/ script.sh`
