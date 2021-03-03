# Maxim Selivanov

### Contscts:

- tel.: +375 29 324 05 49
- e-mail: max_sell@mail.ru
- Minsk 

### About me:

Today my main goal is getting the position of junior Javascript / frontend developer. For this purpose I started studying the RSschool course.

I like to try myself in new fields of activity, gain new knowledge, gain experience and apply it in new directions.

So, my total work experience is over 18 years and it was diverse.

I devoted 10 years to economics, starting as a planning economist and finishing as a chief economist. Then I completely changed my field of activity and became an individual entrepreneur and provided photography services (carried out various types of photography, printed photos, designed photo albums).

To date, I have sold my photo studio and finished photography career in order to completely change the field of activity to information technology.

### Skills:

- Python (entry level)
- C (entry level)
- Javascript/HTML/CSS (in the process of learning)
- Git (in the process of learning) 

### Code example:

```python
myFile = open("input.txt", "r", encoding="utf8")
k = int(myFile.readline())
myList = []
for line in myFile:
    newLine = line.split()
    if int(newLine[-1]) >= 40 and int(newLine[-2]) >= 40 \
            and int(newLine[-3]) >= 40:
        myList.append(newLine)
myFile.close()
myList.sort(key=lambda a: int(a[-1]) + int(a[-2]) + int(a[-3]))
myList.reverse()
konk = []
for i in myList:
    sum = int(i[-1]) + int(i[-2]) + int(i[-3])
    konk.append(sum)
n = len(konk)
def konkurs(n, k, konk):
    if n <= k:
        return 0
    elif konk[k] == konk[0]:
        return 1
    for i in range(k, 0, -1):
        if konk[i] < konk[i - 1]:
            return konk[i - 1]
print(konkurs(n, k, konk))
``` 
