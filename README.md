# arduino_switch

to test switch code


![arduino_switch](https://github.com/octopusoctopus/arduino_switch/blob/master/201510051425137826.png)
출처:코코아팹



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
