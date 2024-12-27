#include "ArduinoGraphics.h"
#include "Arduino_LED_Matrix.h"

ArduinoLEDMatrix matrix;

void setup() {
  Serial.begin(115200);
  matrix.begin();

  matrix.beginDraw();
  matrix.stroke(0xFFFFFFFF);
  matrix.textScrollSpeed(100);
  const char text8[] = "   Isaac_Boyd";//Put text here to be the title on the matrix, it will sroll
  matrix.textFont(Font_4x6);
  matrix.beginText(0, 1, 0xFFFFFF);
  matrix.println(text8);
  matrix.endText(SCROLL_LEFT);//you can change the direction from 'LEFT' to whatever you want!
  delay(1000);
  matrix.beginDraw();

  matrix.stroke(0xFFFFFFFF);
  matrix.textScrollSpeed(100);//Change the scroll, the higher the number the slower it will scroll, the lower the nuber the faster it will scroll.

  // add the text
  const char text3[] = "Hello";//put text here to slide from  the top overtop of the text above
  matrix.textFont(Font_4x6);
  matrix.beginText(0, 1, 0xFFFFFF);
  matrix.println(text3);
  matrix.endText(SCROLL_DOWN);
  matrix.endDraw();
  delay(500);
  matrix.beginDraw();
  matrix.stroke(0xFFFFFFFF);
  matrix.textScrollSpeed(100);
  const char text5[] = "Hello World!";//put text here to scroll, it cooler if the start of the text here and the text above is the same so it looks like it slid down and then scrolled!
  matrix.textFont(Font_4x6);
  matrix.beginText(0, 1, 0xFFFFFF);
  matrix.println(text5);
  matrix.endText(SCROLL_LEFT);
}

void loop() {
  matrix.beginDraw();
  matrix.stroke(0xFFFFFFFF);
  matrix.textScrollSpeed(100);
  const char text2[] = "  Hello World";//put the same text here as the text.
  matrix.textFont(Font_4x6);
  matrix.beginText(0, 1, 0xFFFFFF);
  matrix.println(text2);
  matrix.endText(SCROLL_LEFT);
}
