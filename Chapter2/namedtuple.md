from collections import namedtuple<br/><br/>

Parts = namedtuple('Parts', 'id_num desc cost amount')<br/>
auto_parts = Parts(id_num='1234', desc='Ford Engine',
        cost=1200.00, amount=10)<br/>
print(auto_parts.id_num)<br/><br/>

