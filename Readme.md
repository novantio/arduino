#Arduino simulator 

## basic
software/website : wokwi
### initial pin
```
//using led
char led_pin = 6;

```
### setup begin
initial setup
```
  void setup(){
    Serial.begin(9600); //initial
    //register pin
    pinMode(led_pin,OUTPUT);

  }
```

### loop
for loop main program
```
void loop() {
  //turn om
  digitalWrite(led_pin, HIGH);
  //turn off
  digitalWrite(led_pin, LOW);
}
```

### using button
```
char button_pin=11;
char button_state=0;
void setup(){
    Serial.begin(9600); //initial
    //register pin
    pinMode(button_pin,INPUT);
}

void loop() {
  button_state = digitalRead(button_pin);
  //turn om
  if(button_state==HIGH){
    digitalWrite(led_pin, HIGH);
  //turn off
  }else{
    digitalWrite(led_pin, LOW);
  }
}


```

note:
- analog write for write custom 0-255 , digital write only 0 and 1
- analog read for read custom 0-255, digital read only 0 and 1
- `` Serial.println("printt"); `` for print
