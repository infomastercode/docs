### Thanks link 1 [link](https://devahoy.com/posts/basic-command-line-ubuntu/)

### แสดงข้อมูลของระบบและ Kernel

ใช้สำหรับแสดงรายละเอียดทั้งหมดของระบบ
> uname -i , uname

ใช้สำหรับแสดงจำนวนพื้นที่ฮาดดิสท์
> df

ใช้สำหรับแสดงจำนวนพื้นที่ฮาดดิสท์ โดยใช้หน่วย megabytes และ gigabytes
> df -h

แสดงข้อมูล จำนวน memory ที่ใช้
> free

โชว์รายละเอียดทั้งหมด โปรเซสที่กำลังทำงาน cpu ram อื่นๆ (กด q เพื่อออก)
> top

แสดงรายละเอียด linux ที่ใช้ เวอร์ชั่น และ โค๊ดเนม
> lsb_release -a

### การจัดการ Process

แสดง process ที่กำลังทำงานอยู่
> ps aux

แสดงรายละเอียดโปรเซสของ firefox grep คือ regular expression โดยค้นหาโปรเซสชื่อ firefox
> ps aux | grep firefox

ปิดโปรเซส ตามไอดีที่ระบุ (ไอดีดูได้จาก ps aux)
> kill -9 pid

ปิดโปรเซสของโปรแกรม name
> killall name
