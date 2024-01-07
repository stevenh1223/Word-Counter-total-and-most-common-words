file = open(input('Enter the file name: '), encoding="utf-8")
count = 0
number = 0
dic = dict()
for line in file:
    line = line.rstrip()
    line = line.split()
    if len(line) < 1:
        continue
    for word in line:
        count += 1
        dic[word] = dic.get(word, 0) + 1
print('total words:', count)
common = sorted([(v, k) for k, v in dic.items()], reverse = True )  
print('the 30 most common words:')
for v, k in common[:30]:
    number += 1
    print(str(number) + '. ' + str(k) + ': ' + str(v) + ' times')
