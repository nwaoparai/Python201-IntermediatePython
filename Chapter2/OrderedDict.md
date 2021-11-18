from collections import OrderedDict<br/><br/>

d = {'banana': 3, 'apple':4, 'pear': 1, 'orange': 2}<br/>
new_d = OrderedDict(sorted(d.items()))<br/>
print(new_d)
<br/>
for key in new_d:<br/>
    &ensp;print (key, new&#95;d[key])
