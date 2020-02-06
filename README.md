# digitial-data-processing-using-arduino
int led=12;//input pin of led
int signal=7;//input pin of signal via switch

void setup() {
  pinMode(led,OUTPUT);//declare the led is for output
  pinMode(signal,INPUT);//declare the signal as input
  }
void loop() {
 int val=digitalRead(signal);//measure input signal value 
if (val==1)//if measure value is equal to 1
digitalWrite(led,HIGH);//led pin is on
else 
digitalWrite(led,LOW); //led is off
}
