void setup()
{
  
  pinMode(11,INPUT_PULLUP);
  Serial.begin(9600);
  pinMode(13,OUTPUT); 
  pinMode(12,OUTPUT); 
}
void loop()
{
  Serial.print(digitalRead(11));
  if(digitalRead(11)==LOW)
  {
  digitalWrite(13,HIGH);
  }
  digitalWrite(12,HIGH);
  delay(500);
  digitalWrite(13,LOW);
  digitalWrite(12,LOW);
  delay(500);
}
