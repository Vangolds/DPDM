# บทที่ 1 Introduction
## Data mining คืออะไร
    Data mining (knowledge discovery from data) is extraction of interesting patterns or knowledge from huge amount of data
หรือที่เรียกอีกอย่างหนึ่งว่าการค้นหาความรู้ในฐานข้อมูล ( Knowledge Discovery in Database :KDD) คือกระบวนการที่กระทํากับข้อมูลจํานวนมากเพื่อค้นหารูปแบบและความสัมพันธ์ที่ซ่อนอยู่ในชุดข้อมูลนั้น 
## ทำไม Data Mining ถึงมีความสำคัญ
   The explosive growth of data: from terabytes to petabytes
1. Data collection and data availability
   - Automated data collection tools, database systems, Web, computerized society
2. Major sources of abundant data
   - Business: Web, e-commerce, transactions, stocks, …
   - Science: Remote sensing, bioinformatics, scientific simulation, …
   - Society and everyone: news, digital cameras, YouTube
   
   ในปัจจุบันการทําเหมืองข้อมูลได้ถูกนําไปประยุกต์ใช้ในงานหลายประเภททั้งในด้านธุรกิจที่ช่วยในการตัดสินใจของผู้บริหาร ในด้านวิทยาศาสตร์และการแพทย์รวมทั้งในด้านเศรษฐกิจและสังคม องค์ความรู้ที่สืบค้นได้จากเหมืองข้อมูลจะสามารถทำให้ธุรกิจ สามารถเห็นข้อมูลที่แท้จริงในสิ่งที่ภาคธุรกิจสนใจ เช่น ข้อมูลของลูกค้าที่มีต่อสินค้า  แนวโน้มของผู้บริโภคต่อการซื้อสินค้า
## การดำเนินการของ Knowledge Discovery (KDD) 
   ![image](https://imgur.com/0YmOXO1.jpg)
  - **Database** ฐานข้อมูล คือ กลุ่มของข้อมูลที่ถูกเก็บรวบรวมไว้ โดยมีความสัมพันธ์ซึ่งกันและกัน โดยไม่ได้บังคับว่าข้อมูลทั้งหมดนี้จะต้องเก็บไว้ในแฟ้มข้อมูลเดียวกันหรือแยกเก็บหลาย ๆ แฟ้มข้อมูล
  - **Data cleaning** คือ ขั้นตอนสำหรับการคัดข้อมูลที่ไม่เกี่ยวข้องออกไป
  - **Data integration from multiple sources** คือ ขั้นตอนการรวมข้อมูลที่มีหลายแหล่งให้เป็นข้อมูลชุดเดียวกัน
  - **Warehousing the data** คือ คลังสำหรับเก็บข้อมูลที่รวบรวมข้อมูลจาก Database หรือ ฐานข้อมูลต่างๆ ในองค์กร เพื่อนำข้อมูลเหล่านั้นมาใช้ในการวิเคราะห์ ใช้ประโยชน์ในเชิงธุรกิจ 
  - **Data cube construction**  คือโครงสร้างข้อมูล (Data structure) รูปแบบหนึ่งเพื่อให้วิเคราะห์ข้อมูลได้เร็วขึ้น ซึ่งใช้กับ OLAP โดยส่วนใหญ่ในการทำ OLAP นั้น ได้ใช้ Cube เป็นพื้นฐานในการวิเคราะห์ข้อมูลเป็นหลายมิติ หรือ dimensions นั้นเอง โดยส่วนใหญ่ Cube จะถูกสร้างในส่วนของ Data warehouse 
  - **Data selection for data mining** คือ ขั้นตอนการดึงข้อมูลสำหรับการวิเคราะห์จากแหล่งที่บันทึกไว้
  - **Data mining** เป็นขั้นตอนการค้นหารูปแบบที่เป็นประโยชน์จากข้อมูลที่มีอยู่
  - **Presentation of the mining results**
  - **Patterns and knowledge to be used or stored into knowledge-base** เป็นขั้นตอนการนำเสนอความรู้ที่ค้นพบ โดยใช้เทคนิคในการนำเสนอเพื่อให้เข้าใจ
                เมื่อทำตามขึ้นตอนอย่างถูกต้องก็จะส่งผลให้ข้อมูลที่สืบค้นจากเหมืองข้อมูลมีความถูกต้องแม่นยำและสามารถใช้งานได้จริงตามสิ่งที่ธุรกิจนั้นต้องการ
## Data Mining in Business Intelligence
 BI (Business Intelligence)   คือ  ข้อมูลสรุปที่สามารถนำมาช่วยในการตัดสินใจ หรือตอบคำถามในเชิงธุรกิจให้กับผู้บริหารได้ ดังนั้นระบบ BI ที่ดีจะต้องสามารถ นำเสนอข้อมูลสารสนเทศในเชิงภาพรวมของธุรกิจทั้งหมดขององค์กรได้ 
 ![image](https://imgur.com/VclRiuM.jpg)
 ## KDD Process: A Typical View from ML and Statistics
![image](https://imgur.com/rV5X4TV.jpg)
## Data Mining Function: Classification การจัดหมวดหมู่
- สร้างโมเดลจากข้อมูลที่มีอยู่ 
- เพื่อทำนายเหตุการณ์ที่จะเกิดขึ้นในอนาคต
## Data Mining Function: Cluster Analysis การวิเคราะห์การรวมกลุ่ม 
- แบ่งข้อมูลเป็นหลายๆ กลุ่ม
- อาศัยความคล้ายคลึงกันของข้อมูล
## Association rules
- อาศัยความสัมพันธ์ของข้อมูลที่เกิดร่วมกัน
- สร้างเป็นกฎความสัมพันธ์ เช่น “ซื้อเบียร์แล้วจะซื้อผ้าอ้อมไปด้วย”
## Data Mining Function: Outlier Analysis การวิเคราะห์ข้อมูลที่ผิดปกติ
Outlier analysis

Outlier: A data object that does not comply with the general behavior of the data

Noise or exception? ― One person’s garbage could be another person’s treasure

Methods: by product of clustering or regression analysis, …

Useful in fraud detection, rare events analysis
