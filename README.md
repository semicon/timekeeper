การใช้อ็อบเจ็กต์ Date ใน JavaScript เราสามารถแสดงเขตเวลาเฉพาะประเทศได้ ด้วยเมธอด toLocaleString ในอ็อบเจ็กต์ Date สามารถรับอาร์กิวเมนต์ที่สองซึ่งเป็นอ็อบเจ็กต์ตัวเลือกที่สามารถใช้เขตเวลา  โดยสามารถระบุเขตเวลาที่ต้องการได้ 

ตัวอย่างเช่น หากต้องการแสดงโซนเวลาสำหรับชายฝั่งตะวันออกของสหรัฐอเมริกา:

  
  let date = new Date();
  let options = {timeZone: 'America/New_York'};
  let eastCoastTime = date.toLocaleString('en-US', options);

ตัวอย่างการแสดงโซนเวลาสำหรับประเทศไทย:

  
  let date = new Date();
  let options = {timeZone: 'Asia/Bangkok'};
  let eastCoastTime = date.toLocaleString('th-TH', options);
