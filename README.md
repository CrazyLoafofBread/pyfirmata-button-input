# pyfirmata-button-input
Getting input from a button using arduino and pyfirmata library

This project needs the pyfirmata library, you can install it in terminal by using the command: "pip install pyfirmata".

I will attach a photo of the circuit so you can understand it.
C++ code for the arduino IDE:
// C++ code
//
void setup()
{
  pinMode(13, OUTPUT);
  pinMode(4, INPUT);
}

void loop()
{
  int buttonstate = digitalRead(4);
  if (buttonstate == 1){
    digitalWrite(13, HIGH);
  }
  else{
    digitalWrite(13, LOW);
  }
    delay(10); // Delay a little bit to improve simulation performance
}
