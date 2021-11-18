from collections import defaultdict<br/><br/>


sentence = "The red for jumped over the fence and ran to the zoo for food"<br/>
words = sentence.split(' ')<br/><br/>

d = defaultdict(int)<br/>
for word in words:<br/>
    &ensp;d[word] += 1<br/><br/>

print(d)<br/><br/>

