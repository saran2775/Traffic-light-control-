# Traffic-light-control-
The Traffic Light Control using Arduino is an automated system that controls red, yellow, and green LEDs in a fixed sequence. The Arduino manages signal timing to regulate vehicle movement at road intersections.
int red = 8;
int yellow = 9;
int green = 10;

void setup()
{
  pinMode(red, OUTPUT);
  pinMode(yellow, OUTPUT);
  pinMode(green, OUTPUT);
}

void loop()
{
  // Red light
  digitalWrite(red, HIGH);
  digitalWrite(yellow, LOW);
  digitalWrite(green, LOW);
  delay(5000);

  // Green light
  digitalWrite(red, LOW);
  digitalWrite(yellow, LOW);
  digitalWrite(green, HIGH);
  delay(5000);

  // Yellow light
  digitalWrite(red, LOW);
  digitalWrite(yellow, HIGH);
  digitalWrite(green, LOW);
  delay(2000);
}