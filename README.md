- 👋 Hi, I’m @Zarger-code
- 👀 I’m interested in Coding
- 🌱 I’m currently learning C++ Language
- 💞️ I’m looking to collaborate on Nothing
- 📫 How to reach me discord id = titanshuhaab instagram id = cr7_fan1868
- 😄 Pronouns: If I say that i like Arduino Uno R3 Hammad is going to kill me
- ⚡ Fun fact: i also know the basics of javascript(Node Js) and Python(Python 3.12(64-bit))


```
#include <LiquidCrystal_I2C.h>  //Includes the lcd

LiquidCrystal_I2C lcd(0x27, 16, 2);  //Names the lcd and configures it

void setup(){  //Starts the code once
  Serial.begin(9600);  //Starts the Serial Monitor 
  lcd.backlight();  //Adds backlight to the lcd
  lcd.clear();  //Clears the lcd
}  //Void setup end

void loop(){  //Repeats the code multiple
  while(Serial.available()>0){
  int x = Serial.parseInt();  //Sats x as a Int for Serial.parseInt()
  if(x>=0&&x<=9999999999999999999999999999999999){
  Serial.print("Displayed ");                   
  Serial.println(x);
  lcd.setCursor(0,0);  //Sets the cursor to the start
  lcd.print(x);  //Prints the degrees i tell the lcd to in the Serial Monitor
  Serial.flush(); 
  }
  else{
    Serial.println("Invalid Number");
  }

  }
}  //Void loop end



```

