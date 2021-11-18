from collections import namedtuple<br/><br/>

Parts = namedtuple('Parts', 'id_num desc cost amount')<br/>
auto_parts = Parts(id_num='1234', desc='Ford Engine',
        cost=1200.00, amount=10)<br/>
print(auto_parts.id_num)<br/><br/>

![Screen Shot 11-18-21 at 12 20 PM](https://user-images.githubusercontent.com/46776355/142406214-1a437266-4ab7-4d22-842d-079755d35f61.PNG)
