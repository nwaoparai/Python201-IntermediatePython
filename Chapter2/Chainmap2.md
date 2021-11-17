import argparse<br/>
import os<br/><br/>

from collections import ChainMap<br/><br/>


def main():<br/>
    &emsp;app_defaults = {'username':'admin', 'password':'admin'}<br/><br/>

    &emsp;parser = argparse.ArgumentParser()<br/>
    &emsp;parser.add_argument('-u', '--username')<br/>
    &emsp;parser.add_argument('-p', '--password')<br/>
    &emsp;args = parser.parse_args()<br/>
    &emsp;command_line_arguments = {key:value for key, value in vars(args).items() if value}<br/><br/>

    &emsp;chain = ChainMap(command_line_arguments, os.environ, app_defaults)<br/>
    &emsp;print(chain['username'])<br/><br/>


if &#95;&#95;name&#95;&#95; == '&#95;&#95;main&#95;&#95;':<br/>
    &emsp;main()<br/>
    &emsp;os.environ['username'] = 'test'<br/>
    &emsp;main()
