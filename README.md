This is my first contact with markdown files

<!-- Headings -->

# my title h1

## my title h2

### my title h3

<!-- italic -->

this is an _italic_ text

<!-- strong -->

this is an **strong** text

<!-- striketrough-->

this is ~~striketrough~~ text

<!-- UL unordered list -->

- apple
  - apple 2
- orange
- etc

1. apple
   1. apple 2
2. orange
3. etc

<!-- links -->

[nameofthelink](https://www.google.com)

[nameofthelink](https://www.google.com "Custom title")

> this is a quote

---

---

`console.log('hello world')`

I can use ' to add coding lines to the md file

```python

from Car import \*

class Lane:
width=800
height=40
def **init**(self,x,y,type,numOfVehicles,vehicleSpeed,height):
self.x = x
self.y = y
self.height=height
self.cars=[]
self.carsSpeed=vehicleSpeed
if type==1: #lane of cars
for i in range(numOfVehicles):
if vehicleSpeed>=0:
c=Car(x+i*50,y+height/4,vehicleSpeed)
self.startX = x
#self.startY = y+10
else:
c = Car(x+self.width-i*50, y + height/4, vehicleSpeed)
self.startX = x+self.width
#self.startY = y + 10
self.cars.append(c)

        if type==2: #lane of lorries
            for i in range(numOfVehicles):
                if vehicleSpeed>=0:
                    c=Lorry(x+i*70,y+height/4,vehicleSpeed)
                    self.startX = x
                else:
                    c = Lorry(x+self.width-i*70, y + height/4, vehicleSpeed)
                    self.startX = x+self.width
                self.cars.append(c)

    def isOutsideLimits(self,car):
        if car.x<self.x or car.x>self.x+self.width:
            return True
        return False

    def moveCars(self):
        for c in self.cars:
            c.move()
            if self.isOutsideLimits(c):
                c.x = self.startX

    def draw(self,w):
        w.create_rectangle(self.x,self.y,self.x + self.width, self.y + self.height,fill="gray")
        for c in self.cars:
            c.draw(w)
```

| Title 1 | Title 2 | Title 3 |
| ------- | ------- | ------- |
| data    | data    | data3   |

![visual studio code logo](https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Visual_Studio_Code_1.35_icon.svg/2048px-Visual_Studio_Code_1.35_icon.svg.png)

![visual studio code logo local](vs.png "vs local logo")

<!-- Github Markdown -->

_[x] Task 1
_[x] Task 2
\*[] Task 3
