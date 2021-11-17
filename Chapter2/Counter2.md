from collections import Counter<br/><br/>

counter_one = Counter('superfluous')<br/>
print(counter_one)<br/>
counter_two = Counter('super')<br/>
counter_one.subtract(counter_two)<br/>
print(counter_one)<br/><br/>

![Screen Shot 11-17-21 at 02 21 PM](https://user-images.githubusercontent.com/46776355/142208660-3627f7c4-cb2d-46f6-bce2-af1455f5bd4e.PNG)
