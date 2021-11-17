# Adding Arguments<br/>
import argparse<br/><br/>

def get_args():<br/>
&emsp;""""""<br/>
&emsp;parser = argparse.ArgumentParser(<br/>
&emsp;&emsp;description = "A simple argument parser",<br/>
)<br/><br/>
# required argument
parser.add_argument('-x', action="store", required=True,
&emsp;&emsp;&emsp;help='Help text for option X')




