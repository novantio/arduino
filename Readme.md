#Arduino simulator 
software/website : wokwi
## initial pin
```
//using led
char pinled = 6;

```
## setup begin

```
  void setup(){
    Serial.begin(9600); //initial
    //register pin
    pinMode(pinled,OUTPUT);
    
  }
```

## loop
```
void loop() {
  //turn om
  digitalWrite(pinled, HIGH);
  //turn off
  digitalWrite(pinled, LOW);
}
```
