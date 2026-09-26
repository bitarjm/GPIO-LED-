# GPIO-LED-
int ledPin = 7;  // LED connected to digital pin 7

void setup() {
  pinMode(ledPin, OUTPUT);  // set pin 7 as output
}

void loop() {
  // Step 1: LED ON for 1 second
  digitalWrite(ledPin, HIGH);
  delay(1000);

  // Step 2: Blink LED 5 times in 1 second
  for (int i = 0; i < 5; i++) {
    digitalWrite(ledPin, HIGH);
    delay(100);
    digitalWrite(ledPin, LOW);
    delay(100);
  }

  // Step 3: Force LED OFF
  digitalWrite(ledPin, LOW);

  // Step 4: Infinite loop, LED stays OFF
  while (true) {
    // do nothing
  }
}
