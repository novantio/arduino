#Arduino simulator 
software/website : wokwi
## initial pin
char pinled = 6;

## setup begin

```
  void setup(){
    Serial.begin(9600); #initial
    
    #register pin
    pinMode(pinled,OUTPUT);
    
  }
```

## loop
```
void loop() {
  //turn om
  digitalWrite(ledred, HIGH);
  //turn off
  digitalWrite(ledred, LOW);
}
```
