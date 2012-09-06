int thermR1 = 0;
int pulse = 1;

////--              

void setup()                   
{
  
  pinMode(thermR1, INPUT);      
  Serial.begin(9600);     // инициализация работы с COM-портом
}

void loop()                     
{
  digitalWrite(ledPin, HIGH);   
  Serial.print("H");      // светодиод горит – пишем H
  delay(1000);                  
  digitalWrite(ledPin, LOW);    
  Serial.println("L");    // светодиод погасили – пишем L
  delay(1000);                  
}
