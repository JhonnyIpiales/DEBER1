# DEBER1
ARDUINO
int in=14;
int p=15;
int vector[10]={4,5,6,7,8,9,10,11,12,13};
int a=3;
int jh=3;
int d=14;
int valor=random(4,14);
int cont=1;
void setup()
{
 pinMode(13,OUTPUT);
 pinMode(12,OUTPUT);
 pinMode(11,OUTPUT);
 pinMode(10,OUTPUT);
 pinMode(9,OUTPUT);
 pinMode(8,OUTPUT);
 pinMode(7,OUTPUT);
 pinMode(6,OUTPUT);
 pinMode(5,OUTPUT);
 pinMode(4,OUTPUT);
 pinMode(1,INPUT);
 pinMode(2,INPUT);
 pinMode(3,INPUT);
}

void loop() {
   if(digitalRead(1)==LOW &&digitalRead(2)==HIGH&&digitalRead(3)==LOW)
   {
    while(in>3)
     {
      in=in-2; 
     digitalWrite(in,HIGH);
     delay(200);
     digitalWrite(in,LOW);
     delay(200);
     }
     in=14;
   }
  if(digitalRead(1)==LOW &&digitalRead(2)==HIGH&&digitalRead(3)==HIGH)
   {
    while(p>3)
     {
      p=p-2; 
     digitalWrite(p,HIGH);
     delay(500);
     digitalWrite(p,LOW);
     delay(500);
     }
     p=15;
   }
  if(digitalRead(1)==HIGH &&digitalRead(2)==HIGH&&digitalRead(3)==LOW)
   {
   while(d>=9&&a<=8)
     {
     d=d-1;
     a=a+1; 
     digitalWrite(d,HIGH);
     digitalWrite(a,HIGH);
     delay(500);
     digitalWrite(d,LOW);
     digitalWrite(a,LOW);
     delay(500);
     }
     d=14;
     a=3;
   }
  if(digitalRead(1)==HIGH &&digitalRead(2)==LOW&&digitalRead(3)==HIGH)
   {
 
     digitalWrite(valor,HIGH);
     delay(500);
     digitalWrite(valor,LOW);
     delay(500);
     valor= random(4,14); 
   }
 if(digitalRead(1)==HIGH &&digitalRead(2)==HIGH&&digitalRead(3)==HIGH)
   {
    for(;cont<6;cont++)
    {
    while(jh<=14)
    {
      jh=jh+1;
      digitalWrite(jh,HIGH);
      delay(200);
      digitalWrite(jh,LOW);
      delay(200);
     }
     jh=3;
    }
   }

   
}
