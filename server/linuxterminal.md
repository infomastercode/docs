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

### การจัดการโฟลเดอร์

คำสั่งเปลี่ยน directory
> cd

เปลี่ยน directory ไปที่ root
> cd /

ใช้สำหรับแสดง directory ปัจจุบัน
> pwd

ใช้สำหรับก็อปปี้ ไฟล์/โฟลเดอร์
> cp

ใช้สำหรับสร้างโฟลเดอร์
> mkdir folder1

ลบโฟลเดอร์ folder1 (เฉพาะfolder ที่ไม่มีไฟล์ข้างใน)
> rmdir folder1

ลบโฟลเดอร์ folder1 และไฟล์ข้างในทั้งหมด
> rm -R folder1

### การจัดการไฟล์

สร้างไฟล์ file1.txt
> touch file1.txt

แสดงนามสกุลของ file1
> file file1

แสดงรายละเอียดข้างใน file1.txt
> cat file1.txt

เหมือนคำสั่ง cat แต่ต่างกันที่ สามารถเลื่อน scroll bar ได้
> less file1.txt

ก็อปปี้ file1 และสร้าง file2
> cp file1 file2

ลบ file1
> rm file1






















