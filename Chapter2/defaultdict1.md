from collections import defaultdict<br/><br/>


sentence = "The red for jumped over the fence and ran to the zoo for food"<br/>
words = sentence.split(' ')<br/><br/>

d = defaultdict(int)<br/>
for word in words:<br/>
    &ensp;d[word] += 1<br/><br/>

print(d)<br/><br/>

![Screen Shot 11-18-21 at 09 50 AM](https://user-images.githubusercontent.com/46776355/142383000-d5df2e94-02f6-49c3-90cb-10fec832868a.PNG)
