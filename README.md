# fastestDigitialWrite
faster digitalWrite replacement for Arduino.

usage :
 just #include "fastestDigitalRW.hpp" like below:

-----------------------------------------------
#include <Arduino.h>
#include "fastestDigitalRW.hpp"

#define DOUT_PIN (10)

void setup() {
  pinMode(DOUT_PIN, OUTPUT);
  pinMode(DIN_PIN, INPUT);
}

void loop() {
  for(;;) {
    fastestDigitalWrite(DOUT_PIN, HIGH);  // 35 times faster than digitalWrite()!!!
    fastestDigitalWrite(DOUT_PIN, LOW);
  }
}
-----------------------------------------------
