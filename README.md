void setup(){
  pinMode(6, INPUT);
  pinMode(13, OUTPUT);
  pinMode(12, OUTPUT);
}

void loop(){
  	int movimento = digitalRead(6);
  
  if (movimento) {
    digitalWrite(13, HIGH);
    digitalWrite(12, HIGH);
  	delay(2000);
  } 
  else { 
  	digitalWrite(13, LOW);
    digitalWrite(12, LOW);
  }
}
