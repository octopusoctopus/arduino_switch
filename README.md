# arduino_switch

to test switch code

```cpp
void setup() {
  // put your setup code here, to run once: 
  Serial.begin(9600);
  pinMode(13,OUTPUT);
  pinMode(3,INPUT_PULLUP);
  
}

void loop() {
  // put your main code here, to run repeatedly:
  int value;
  
  value=digitalRead(3);
  
  if(value==0){
    //led on
    digitalWrite(13,HIGH);
    Serial.println("LED ON");
  }else{
    //led off
    digitalWrite(13,LOW);
  }

}

```
