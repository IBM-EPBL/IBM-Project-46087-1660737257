

int trigPin = 13;
int echoPin = 12;
int led = 11;


void setup() {
Serial.begin (9600);
pinMode(trigPin, OUTPUT);
pinMode(echoPin, INPUT);
pinMode(led, OUTPUT);
  pinMode(2, INPUT);
  Serial.begin(9600);
  pinMode(13, OUTPUT);
}


void loop() {
  
long duration, distance;
digitalWrite(trigPin, LOW);
delayMicroseconds(2);
digitalWrite(trigPin, HIGH);
delayMicroseconds(10);
digitalWrite(trigPin, LOW);
duration = pulseIn(echoPin, HIGH);

distance = (duration/2)/29.1;
if (distance < 10) { // This is where the LED On/Off happens hen a duration of 58microseconds corrsponds to distance of 2cm
digitalWrite(led,HIGH); // When the Red condition is met, the Green LED should turn off
}
  
else {
digitalWrite(led,LOW);
}
Serial.println(digitalRead(2));
  if (digitalRead(2) == 1) {
    digitalWrite(13, HIGH);
  } else {
    digitalWrite(13, LOW);
  }
  delay(10);
 // Delay a little bit to improve simulation performance
}
  

