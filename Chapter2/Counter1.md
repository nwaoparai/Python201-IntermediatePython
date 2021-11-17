from collections import Counter<br/><br/>

Counter('superfluous')<br/>
Counter({'u': 3, 's': 2, 'e': 1, 'l': 1, 'f': 1, 'o': 1, 'r': 1, 'p': 1})<br/>
counter = Counter('superfluous')<br/>
print(counter['u'])<br/>
print(list(counter.elements()))<br/>
print(list(counter.most_common(2)))<br/><br/>

![Screen Shot 11-17-21 at 02 09 PM](https://user-images.githubusercontent.com/46776355/142206794-62951f42-4849-4be3-8d8a-688f64bede71.PNG)
