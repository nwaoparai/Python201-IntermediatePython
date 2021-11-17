from collections import Counter<br/><br/>

counter_one = Counter('superfluous')<br/>
print(counter_one)<br/>
counter_two = Counter('super')<br/>
counter_one.subtract(counter_two)<br/>
print(counter_one)
