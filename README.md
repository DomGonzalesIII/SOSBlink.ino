/*
  SOS Blink

  Modified the Blink example to flash "S.O.S." in morse code.

  Written on 1/26/18
*/

// the setup function runs once when you press reset or power the board
void setup() {
  pinMode(LED_BUILTIN, OUTPUT);      // initialize digital pin LED_BUILTIN as an output
}
 
  
// S blink
int blinks = 0;                      // while loop counter
while (blinks != 3) {
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(450);                        // wait for about half a second; number's are odd because this blink rate looked better
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(450);                        // wait for about half a second
  blinks ++;                         // increase blinks counter by 1
  }

// O blink
blinks = 0;                          // while loop counter, reset to 0
while (blinks != 3) {
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(950);                        // wait for about a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(950);                        // wait for about a second
  blinks ++;                         // increase blinks counter by 1
  }

// Second S blink, then a pause
blinks = 0;                          // while loop counter, reset to 0
while (blinks != 3) {              
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(450);                        // wait for about half a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(450);                        // wait for about half a second
  blinks ++;                         // increase blinks counter by 1
  }
 
  delay(950);                        // wait for about half a second before looping the full S.O.S. blink set again
