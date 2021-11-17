import argparse<br/>
import os<br/><br/>

from collections import ChainMap<br/><br/>


def main():<br/>
    &emsp;app_defaults = {'username':'admin', 'password':'admin'}<br/><br/>

    parser = argparse.ArgumentParser()<br/>
    parser.add_argument('-u', '--username')<br/>
    parser.add_argument('-p', '--password')<br/>
    args = parser.parse_args()<br/>
    command_line_arguments = {key:value for key, value in vars(args).items() if value}<br/><br/>

    chain = ChainMap(command_line_arguments, os.environ, app_defaults)<br/>
    print(chain['username'])<br/><br/>


if &#95;&#95;name&#95;&#95; == '&#95;&#95;main&#95;&#95;':<br/>
    main()<br/>
    os.environ['username'] = 'test'<br/>
    main()
