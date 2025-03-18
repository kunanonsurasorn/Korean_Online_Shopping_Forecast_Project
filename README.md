# **โปรเจคการพยากรณ์การซื้อสินค้าประเภทเสื้อผ้าและเครื่องแต่งกายในประเทศเกาหลีใต้**

## 1. วัตถุประสงค์ 

     1.1 เพื่อพยากรณ์การซื้อสินค้าประเภทเสื้อผ้าและเครื่องแต่งกายในอนาคต
 
     1.2 เพื่อหาโมเดลที่เหมาะสมสำหรับการพยากรณ์

## 2. ชุดข้อมูล

     2.1 ชุดข้อมูลที่ใช้มาจากหน่วยงานสถิติของประเทศเกาหลีใต้ (Korean Statistical Information Service) 
 
     2.2 เว็บไซต์ของหน่วยงานสถิติประเทศเกาหลีใต้ : https://kosis.kr/eng/

## 3. ภาษาที่ใช้ในการเขียนโปรแกรม

     ภาษาที่ใช้ในการเขียนโปรแกรมคือ Python

## 4. Python Libraries ที่ใช้ในการทำโปรเจค

     4.1 Pandas
 
     4.2 Matplotlib
 
     4.3 Sktime

## 5. โมเดลที่ใช้ในการทำโปรเจค
    
     โมเดลที่ใช้ในการทำโปรเจคคือ ExponentialSmoothing()

## 5. ผลลัพท์

 ### 5.1 การพยากรณ์สินค้าประเภท Clothing
 
       5.1.1 Parameter ของโมเดลก่อนปรับปรุงประกอบด้วย trend = 'add' , seasonal = 'add' , sp = 12 , smoothing_level = 0, smoothing_trend = 0, smoothing_seasonal = 0
   
       5.1.2 ค่า Mean Absolute Error ของโมเดลก่อนคือ 94618.8294
   
       5.1.3 ค่า Mean Absolute Percentage Error ของโมเดลก่อนคือ 0.0528
   
       5.1.5 Parameter ของโมเดลหลังปรับปรุงประกอบด้วย trend = 'add' , seasonal = 'add' , sp = 12 , smoothing_level = 0, smoothing_trend = 0.5, smoothing_seasonal = 0.5
   
       5.1.6 ค่า Mean Absolute Error ของโมเดลหลังคือ 87163.5649
   
       5.1.7 ค่า Mean Absolute Percentage Error ของโมเดลหลังคือ 0.0494
   
 ### 5.2 การพยากรณ์สินค้าประเภท Footwear
 
       5.1.1 Parameter ของโมเดลก่อนปรับปรุงประกอบด้วย trend = 'add' , seasonal = 'add' , sp = 12 , smoothing_level = 0, smoothing_trend = 0, smoothing_seasonal = 0
   
       5.1.2 ค่า Mean Absolute Error ของโมเดลก่อนคือ 51528.2368
   
       5.1.3 ค่า Mean Absolute Percentage Error ของโมเดลก่อนคือ 0.1687
   
       5.1.5 Parameter ของโมเดลหลังปรับปรุงประกอบด้วย trend = 'add' , seasonal = 'add' , sp = 12 , smoothing_level = 0.5, smoothing_trend = 0, smoothing_seasonal = 1.0
   
       5.1.6 ค่า Mean Absolute Error ของโมเดลหลังคือ 44596.6816
   
       5.1.7 ค่า Mean Absolute Percentage Error ของโมเดลหลังคือ 0.1435

 ### 5.3 การพยากรณ์สินค้าประเภท Fashion และ Accessories
 
       5.1.1 Parameter ของโมเดลก่อนปรับปรุงประกอบด้วย trend = 'add' , seasonal = 'add' , sp = 12 , smoothing_level = 0, smoothing_trend = 0, smoothing_seasonal = 0
   
       5.1.2 ค่า Mean Absolute Error ของโมเดลก่อนคือ 17063.8232
   
       5.1.3 ค่า Mean Absolute Percentage Error ของโมเดลก่อนคือ 0.0537
   
       5.1.5 Parameter ของโมเดลหลังปรับปรุงประกอบด้วย trend = 'add' , seasonal = 'add' , sp = 12 , smoothing_level = 0, smoothing_trend = 0, smoothing_seasonal = 0
   
       5.1.6 ค่า Mean Absolute Error ของโมเดลหลังคือ 17063.8232
   
       5.1.7 ค่า Mean Absolute Percentage Error ของโมเดลหลังคือ 0.0537
   
   
