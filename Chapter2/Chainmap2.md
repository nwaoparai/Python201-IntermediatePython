import argparse<br/>
import os<br/><br/>

from collections import ChainMap<br/><br/>


def main():<br/>
    &ensp;app_defaults = {'username':'admin', 'password':'admin'}<br/>
    &ensp;parser = argparse.ArgumentParser()<br/>
    &ensp;parser.add_argument('-u', '--username')<br/>
    &ensp;parser.add_argument('-p', '--password')<br/>
    &ensp;args = parser.parse_args()<br/>
    &ensp;command_line_arguments = {key:value for key, value in vars(args).items() if value}<br/><br/>
    &ensp;chain = ChainMap(command_line_arguments, os.environ, app_defaults)<br/>
    &ensp;print(chain['username'])<br/><br/>


if &#95;&#95;name&#95;&#95; == '&#95;&#95;main&#95;&#95;':<br/>
    &ensp;main()<br/>
    &ensp;os.environ['username'] = 'test'<br/>
    &ensp;main()<br/><br/>
    
![Screen Shot 11-17-21 at 01 10 PM](https://user-images.githubusercontent.com/46776355/142198494-95b6c203-a33f-485d-8e6d-fb804b537dfd.PNG)

