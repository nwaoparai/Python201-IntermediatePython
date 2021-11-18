from collections import defaultdict<br/><br/>


my_list = [(1234, 100.23), (345, 10.45), (1234, 75.00),
(345, 222.66), (678, 300.25), (1234, 35.67)]<br/><br/>

d = defaultdict(list)<br/>
for acct_num, value in my_list:<br/>
    &ensp;d[acct_num].append(value)<br/><br/>

print(d)
<br/><br/>
![Screen Shot 11-18-21 at 10 33 AM](https://user-images.githubusercontent.com/46776355/142389320-04b09301-0693-4449-afe3-077a433d1223.PNG)
