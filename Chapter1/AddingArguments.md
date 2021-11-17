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

if &#95;&#95;name&#95;&#95;=='&#95;&#95;main&#95;&#95;':<br/>
&emsp;get_args()
<br/><br/>
![Screen Shot 11-16-21 at 03 30 PM](https://user-images.githubusercontent.com/46776355/142159168-8b2b22c3-f922-48ae-aabc-0de04affb1d6.PNG)





