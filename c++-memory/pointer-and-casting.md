# pointer & casting

## พ้อยเตอร์คืออะไร

1. พ้อยเตอร์คือ ตัวแปรที่ใช้เก็บตำแหน่งที่อยู่ของตัวเเปร เช่น 0x0123abcde
2. (type \* ) คือชื่อประเภทตัวแปร ตามด้วย \* เป็นการบ่งบอกว่าคือ pointer&#x20;

## Type conversions หรือ การ Casting ตัวแปร

การ Casting ตัวแปรก็คือ การเปลี่ยนตัวแปรให้อยู่ในประเภทที่เราต้องการ

```
float a = (float)b;
```

ตัวยอ่างข้างต้นคือการ Casting ให้ตัวแปร b มีประเภทเป็น float

## การอ่านค่าจากตำแหน่งที่อยู่ของ Pointer

การอ่าน Value ของตัวแปรพ้อยเตอร์ ที่มีการเก็บค่าตำแหน่งที่อยู่ของตัวแปรสามารถทำได้ดังนี้

```
int health = 100;
int * addressOfHealth = &health;
int valueOfHealth = *addressOfHealth; 

printf("health: %i\n", health);
printf("addressOfHealth: %p\n", addressOfHealth);
printf("valueOfHealth: %.2f\n", valueOfHealth);

health: 100
addressOfHealth: 00000009D54FF624
valueOfHealth: 100.00
```
