# Arduino LM35 Temperature Monitor

## Mo ta
Du an su dung Arduino Uno va 3 cam bien LM35 de do nhiet do tai 3 vi tri khac nhau (chan A0, A1, A2). Du lieu duoc xuat ra cong Serial duoi dang JSON. Kem theo la ung dung C# Windows Forms hien thi do thi nhiet do thoi gian thuc va file mo phong Proteus.

## Tinh nang
- Doc nhiet do tu 3 cam bien LM35 (do phan giai 10mV/do C).
- Xuat du lieu dang JSON qua Serial (9600 baud).
- Ung dung C# ve bieu do 3 duong nhiet do theo thoi gian.
- Mo phong mach dien tren Proteus.
- Ho tro .gitignore loai tru file nhi phan (.exe, .dll, .hex, .pdsbak).

## Phan cung
| Thanh phan      | So luong | Ghi chu                         |
|-----------------|----------|---------------------------------|
| Arduino Uno     | 1        | Co the dung Mega/Nano           |
| LM35            | 3        | Cam bien nhiet do (10mV/do C)   |
| Breadboard      | 1        | 400 hoac 830 diem               |
| Day noi         | ~10      | Ket noi cac chan                |
| Nguon 5V        | 1        | Tu USB Arduino hoac adapter     |

## Huong dan su dung
1. **Nap code Arduino**  
   Mo file `firmware/LM35_TempReader/LM35_TempReader.ino` bang Arduino IDE, chon board va cong COM, sau do nhan Upload.
2. **Xem du lieu tho**  
   Mo Serial Monitor (9600 baud) de quan sat cac dong JSON.
3. **Chay ung dung C#**  
   Vao thu muc `pc_app/bin/Release/` chay file `TemperatureGraph.exe` (yeu cau .NET Framework 4.7.2). Chon dung cong COM, nhan "Start" de ve bieu do.
4. **Mo phong Proteus**  
   Mo file `simulation/LM35_3chan.pdsprj` (neu co) de chay mo phong.

## Cau truc thu muc
- Arduino_LM35_TempMonitor/
  - firmware/
    - MYMAIN/
  - pc_app/
    - WindowsFormsApplication1/
  - docs/
  - libs/
  - simulation/
  - .gitignore
  - README.md

## Tac gia
[Nguyen Tran Trung Linh](https://raumaniac.github.io) - Sinh vien PTIT
