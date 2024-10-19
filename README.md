
#Este es el codigo puesto en el IDE de Arduino
int x;

void setup() {
  Serial.begin(115200);
  Serial.setTimeout(1);
}

void  loop() {
  while (!Serial.available());
  x = Serial.readString().toInt();
  Serial.print(x + 1);
}
