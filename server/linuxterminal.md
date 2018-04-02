### Thanks link 1 [link](https://devahoy.com/posts/basic-command-line-ubuntu/)

### แสดงข้อมูลของระบบและ Kernel

ใช้สำหรับแสดงรายละเอียดทั้งหมดของระบบ
> uname -i , uname, uname -a

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

### ls Option ใช้สำหรับ แสดงรายชื่อไฟล์และโฟลเดอร์

โชว์ไฟล์และโฟลเดอร์
> ls

โชว์ไฟล์และโฟลเดอร์รวม hidden files ด้วย
> ls -a

โชว์ลิสท์แบบยาว มีรายละเอียด permission รวมอยู่ด้วย
> ls -l

โชว์ลิสท์โดยเรียง จากขนาดของไฟล์และโฟลเดอร์
> ls -s

เรียงตามวันที่แก้ไขล่าสุด
> ls -t

โชว์ลิสท์รายชื่อ โดยเรียงบรรทัดละ 1 ชื่อ
> ls -1

แสดงรายชื่อ แบบมีไฮไลท์สี
> ls --color

### การจัดการ Package

ทำการ update รายชื่อpackage ใน lists (เหมือนกับการ check update)
> sudo apt-get update

ทำการ upgrade โปรแกรม ที่มีเวอร์ชั่นใหม่ ให้อัพเดท
> sudo apt-get upgrade

ติดตั้งโปรแกรม
> sudo apt-get install packagename

สำหรับแก้ไข package ที่มีปัญหา กรณีเกิด “unmet dependences”
> sudo apt-get -f install

ลบ package ชื่อname
> sudo apt-get remove name

เหมือนกับ remove แต่จะลบ ไฟล์คอนฟิคด้วย
> sudo apt-get purge name

เพิ่ม repository (ต้องลง python-software-properties ก่อน)
> sudo add-apt-repository ppa:name

### การจัดการ File Permission

เปลี่ยนโหมดไฟล์เป็น 775
> chmod 775 file1

เปลี่ยน folder1 เป็น 777
> chmod 777 folder1

เปลี่ยนสิทธิ์การเข้าถึงของ file1
> chown user:group file1

### อื่นๆ

แสดงรายละเอียด network
> ifconfig

ใช้สำหรับเปิด file manager (sudo เพื่อเปิดในฐานะ root)
> nautilus 
> sudo nautilus

ดาวน์โหลดไฟล์ ตามที่ระบุใน url_file
> wget url_file

ดาวน์โหลดไฟล์ ตามที่ระบุใน url_file (แตกต่างจาก wget เล็กน้อย)
> curl url_file

ดูเวลาที่ user ใช้
> uptime

## create new user

create a new user
> adduser [myuser]

check to make sure they were added
> id [myuser]

Add the user to the sudo group
> usermod -aG sudo [myuser]

Login as that as user
> sudo su - [myuser]















































