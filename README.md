# fan
void setup()   
{   
pinMode(2,OUTPUT);  
pinMode(5,OUTPUT);  
pinMode(6,OUTPUT);  
}  
  
void loop()   
{  
fowr(200);  
delay(1000);  
brake();  
delay(2000);  
rev(200);  
delay(1000);  
}  
void fowr(int f)   
{   
analogWrite (5,f);  
analogWrite (6,0);  
}  
void rev(int r)   
{  
analogWrite (5,0);  
analogWrite (6,r);  
}  
void brake()  
{  
analogWrite (5,255);  
analogWrite (6,255);  
}  
