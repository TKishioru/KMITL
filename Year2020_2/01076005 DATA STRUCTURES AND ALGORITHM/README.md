# Python Tutorial
แหล่งที่มาในการสืบค้นข้อมูล >> [คลิก](https://www.w3schools.com/python/default.asp) <<

## ชนิดข้อมูล
- อักขระ & ข้อความ
  > Text Type:	str
- ตัวเลข
  > Numeric Types:	int, float, complex
- กลุ่มข้อมูล (เปรียบเหมือน Array)
  > Sequence Types:	list, tuple, range
  > Mapping Type:	dict
  > Set Types:	set, frozenset
- จริง/เท็จ
  > Boolean Type:	bool
- อื่นๆ

## ประกาศตัวแปร
ภาษาไพธอนเป็นอีกภาษาหนึ่งที่ไม่จำเป็นต้องประกาศชนิดตัวแปร 
``` py
txt = "สามารถประกาศตัวแปรมาได้เลย ซึ่งชนิดข้อมูลของตัวแปรจะยึดตามข้อมูลที่มีอยู่ในตัวแปร" ##ตัวอย่างเป็นชนิดข้อความ
num01 = 2565
num02 = 7.7
``` 

*เว้น* ชนิด กลุ่มข้อมูล

เช่น
``` py
# กลุ่มข้อมูล ประเภท list

lst01 = []
lst02 = list()

```
## OUTPUT
``` py
# ประกาศเพียงข้อความ
print("ข้อความ")

# ประกาศข้อความ + ตัวแปร
num = 2565
print("ข้อความ", num) ## Output : ข้อความ 2565

# ประกาศตัวแปร + ตัวแปร
print(num , num) ## Output : 2565 2565

``` 
*หากสังเกต การที่เราใช้คำสั่ง print มาเรื่อยๆทุกครั้ง จะมีการขึ้นบรรทัดใหม่ให้ ซึ่งในภาษาซี จะเป็นการเพิ่มข้อความไปทางด้านขวา*
**เทคนิค**ที่จะเพิ่มข้อความไปด้านขวา `print("ข้อความ", end="")` 

## INPUT
``` py
##จะถูกป้อนมาเป็นชนิด str. ทั้งหมดก่อน แม้ว่า..จะใส่ตัวเลข
## สามารถใส่หลายค่าได้เลย

inp = input("ข้อความที่จะไว้โชว์เฉยๆ") 
``` 

## OPERATOR
**แนะนำเพียงพื้นฐาน**
- `+` บวก
- `-` ลบ
- `*` คูณ ----> หากเป็น "ข้อความ" * num จะเป็นการซ้ำข้อความตามจำนวน
- `/` หาร(เป็นทศนิยม)
- `%` หารเอาเศษ
- `and` ค่าจะเป็นจริง เมื่อเงื่อนไขเป็นจริงทั้งคู่
- `or` ค่าจะเป็นเท็จ เมื่อเงื่อนไขเป็นเท็จทั้งคู่
- อื่นๆ

## IF - ELSE
คำสั่งเงื่อนไข || ห้าม tab ผิด ไม่อย่างงั้นเกิด error
``` py
# If
if x == 25:
  print("True")
  
# If-else
if x == 25:
  print("True")
else:
  print("false")
  
# If-else if
if x == 25:
  print("True, 25")
elif x == 10:
  print("True, 10")
else:
  print("false")
  
## ไม่มี switch case เหมือนภาษาซี
## สามารถซ้อนเงื่อนไขได้เลย
```
## LOOP
คำสั่งทำซ้ำเมื่อเงื่อนไขเป็นจริง || ห้าม tab ผิด ไม่อย่างงั้นเกิด error
``` py
# While loop
## ไม่มี do...while เหมือนภาษาซี
while i < 5:
  print(i)

# For loop
for i in range(0,5):
  print(i)
  
##ฟังก์ชัน range(จุดเริ่มต้น, จุดสิ้นสุด - 1, เพิ่มค่ารอบละ i)
##ใช้ `break` เมื่อต้องการออกจากลูป (ควรตั้งเงื่อนไข)
``` 
## ARRAY : LIST
``` py
inp = input("Enter Number") ##Input : 1 2 3 4 5
print(inp[0]) ##ข้อมูลในตำแหน่งที่ 0 : ["1 2 3 4 5"]

#ถ้าใช้ฟังก์ชันแยกส่วน spilt()
## สามารถระบุได้ว่าจะแยกด้วยอะไร เช่น spilt(",") เจอ , ให้แยกส่วน
inp = input("Enter Number").spilt() ##Input : 1 2 3 4 5
print(inp[0]) ##ข้อมูลในตำแหน่งที่ 0 : ["1"]

inp = input("Enter Number").spilt(",") ##Input : 1,2 3,4 5
print(inp[0]) ##ข้อมูลในตำแหน่งที่ 0 : ["1"]
print(inp[1]) ##ข้อมูลในตำแหน่งที่ 1 : ["2 3"]
print(inp[2]) ##ข้อมูลในตำแหน่งที่ 2 : ["4 5"]

##จำนวน index/ขนาด
n = len(inp)
``` 