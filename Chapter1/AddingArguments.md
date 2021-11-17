<!-- Adding Arguments -->
<br/>
import argparse<br/><br/>

def get_args():<br/>
&emsp;""""""<br/>
&emsp;parser = argparse.ArgumentParser(<br/>
&emsp;&emsp;description = "A simple argument parser",<br/>
&emsp;)<br/><br/>

<!-- required argument -->
&emsp;parser.add_argument('-x', action="store", required=True,<br/>
&emsp;&emsp;&emsp;help='Help text for option X')<br/><br/>

<!-- optional arguments -->
<br/>
&emsp;parser.add_argument('-y', help='Help text for option Y', default=False)<br/>
&emsp;parser.add_argument('-z', help='Help text for option Z', type=int)<br/>
&emsp;print(parser.parse_args())<br/><br/>

if __name__=='__main__':<br/>
&emsp;get_args()





