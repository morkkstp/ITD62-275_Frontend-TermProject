# ITD62-275_Frontend-Term-Project
# อธิบายเกี่ยวกับ Term Project
เป็น term project เกี่ยวกับระบบจองเต็นท์สำหรับพนักงาน โดยพนักงานเป็นคนกรอกข้อมูลต่างๆของนักท่องเที่ยวที่เดินเข้าไปจองเต็นท์กับพนักงาน

วัตถุประสงค์ของการทำระบบจองเต็นท์สำหรับพนักงาน คือ เพื่อตอบสนองกลุ่มใช้งานของพนักงานในการให้บริการหน้าเคาน์เตอร์หรือหน่วยบริการ เพื่อจัดการให้การจองเป็นระบบมากยิ่งขึ้นและจัดเก็บข้อมูลได้ครบถ้วน อาทิ วันเริ่มจอง, วันสิ้นสุดการจอง, ข้อมูลผู้จอง ชื่อ-สกุล-เบอร์โทร-เลขบัตรประชาชน-ที่อยู่, การเช่าอุปกรณ์ที่มีให้บริการจากทางร้าน, และการบันทึกการชำระเงินและเก็บหลักฐานการชำระเงิน, นอกจากนี้ระบบยังมีความสามารถในการแก้ไข และลบ อีกทั้งยังสามารถส่งออกข้อมูลเป็นไฟล์ Excel ได้อีกด้วย
# อธิบายเกี่ยวกับ Data Dictionary
id คือ Key ที่เก็บค่า id ของนักท่องเที่ยว
firstname คือ Key ที่เก็บชื่อจริงของนักท่องเที่ยว
lastname คือ Key ที่เก็บนามสกุลของนักท่องเที่ยว
phonenumber คือ Key ที่เก็บเบอร์โทรศัพท์ของนักท่องเที่ยว
idcard คือ Key ที่เก็บหมายเลขบัตรประชาชนของนักท่องเที่ยว
address คือ Key ที่เก็บที่อยู่ของนักท่องเที่ยว
subdistrict คือ Key ที่เก็บตำบลของนักท่องเที่ยว
district คือ Key ที่เก็บอำเภอของนักท่องเที่ยว
province คือ Key ที่เก็บจังหวัดของนักท่องเที่ยว
postcode คือ Key ที่เก็บรหัสไปรษณีย์ของนักท่องเที่ยว
checkin คือ Key ที่เก็บวันเข้าพักของนักท่องเที่ยว
checkout คือ Key ที่เก็บวันออกของนักท่องเที่ยว
payment คือ Key ที่เก็บหลักฐานการโอนเงินของนักท่องเที่ยว
zone คือ Key ที่เก็บจุดที่นักท่องเที่ยวจองและทำการกางเต็นท์
equipment คือ Key ที่เก็บการเช่ายืมอุปกรณ์ที่อำนวยความสะดวกต่างๆ ซึ่งมีให้เลือกหลากหลาย ดังนั้นแล้วจึงต้องจัดเก็บเป็น JSON Object ซึ่งมีข้อมูลดังนี้
- hanginglamp คือ Key ที่เก็บการเช่ายืมโคมไฟห้อยของนักท่องเที่ยว ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 40 บาท
- torch คือ Key ที่เก็บการเช่ายืมไฟฉายของนักท่องเที่ยว ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 20 บาท
- illumination คือ Key ที่เก็บการเช่ายืมไฟส่องสว่างของนักท่องเที่ยว ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 80 บาท
- electricity คือ Key ที่เก็บการเช่ายืมไฟฟ้าของนักท่องเที่ยว ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 150 บาท
- privateBathroom คือ Key ที่เก็บการเช่ายืมห้องน้ำส่วนตัวของนักท่องเที่ยว ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 50 บาท
- sharedBathroom คือ Key ที่เก็บการเช่ายืมห้องน้ำรวมของนักท่องเที่ยว ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 20 บาท
- charCoalGrill คือ Key ที่เก็บการเช่ายืมเตาปิ้งแบบถ่านของนักท่องเที่ยว ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 50 บาท
- electricToaster คือ Key ที่เก็บการเช่ายืมเตาปิ้งแบบไฟฟ้าของนักท่องเที่ยว ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 60 บาท
- wifi คือ Key ที่เก็บการเช่ายืม WIFI ของนักท่องเที่ยว ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 50 บาท
- foldingTablehigh คือ Key ที่เก็บการเช่ายืมโต๊ะพับสูงของนักท่องเที่ยว ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 30 บาท
- campingSleepingBag คือ Key ที่เก็บการเช่ายืมถุงนอนตั้งแคมป์ของนักท่องเที่ยว ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 50 บาท
- foldingChair คือ Key ที่เก็บการเช่ายืมเก้าอี้พับของนักท่องเที่ยว ซึ่งจะเก็บเป็นราคา โดยเก็บราคาที่ 30 บาท
# รายชื่อสมาชิก
1. 64114069 เศรษฐพงษ์ เคียนเขา 
2. 64109010 พงษ์นภัส ชูช่วย
3. 64111412 เมธานุสรณ์ สุทธิรัตน์
