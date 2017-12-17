
//library

#include <Arduino_FreeRTOS.h>
#include <NewPing.h>

//+++++++++++++++++++++++++++++++++++++

//inisialisasi pin dan task
 
#define SONAR_NUM 8
#define MAX_DISTANCE 200
#define lednumb 8
NewPing sonar[SONAR_NUM] = {     
  NewPing(36, 37, MAX_DISTANCE), 
  NewPing(38, 39, MAX_DISTANCE),
  NewPing(40, 41, MAX_DISTANCE),
  NewPing(42, 43, MAX_DISTANCE),
  NewPing(44, 45, MAX_DISTANCE),
  NewPing(46, 47, MAX_DISTANCE),
  NewPing(48, 49, MAX_DISTANCE),
  NewPing(50, 51, MAX_DISTANCE)
};

void TaskUS1(void *pvParameters);
void TaskUS2(void *pvParameters);
void TaskUS3(void *pvParameters);
void TaskUS4(void *pvParameters);
void TaskUS5(void *pvParameters);
void TaskUS6(void *pvParameters);
void TaskUS7(void *pvParameters);
void TaskUS8(void *pvParameters);

int led [lednumb] = {
  3,11,5,6,7,8,9,10
};
//+++++++++++++++++++++++++++++++++++++


void setup() {
  
  xTaskCreate(
    TaskUS1
    ,  (const portCHAR *) "Ultrasonic1"
    ,  128  // Stack size
    ,  NULL
    ,  5  // Priority
    ,  NULL );

    
  xTaskCreate(
    TaskUS2
    ,  (const portCHAR *) "Ultrasonic2"
    ,  128  // Stack size
    ,  NULL
    ,  5  // Priority
    ,  NULL );

    
  xTaskCreate(
    TaskUS3
    ,  (const portCHAR *) "Ultrasonic3"
    ,  128  // Stack size
    ,  NULL
    ,  5  // Priority
    ,  NULL );

    
  xTaskCreate(
    TaskUS4
    ,  (const portCHAR *) "Ultrasonic4"
    ,  128  // Stack size
    ,  NULL
    ,  5  // Priority
    ,  NULL );
    
  xTaskCreate(
    TaskUS5
    ,  (const portCHAR *) "Ultrasonic5"
    ,  128 // Stack size
    ,  NULL
    ,  5  // Priority
    ,  NULL );

    
  xTaskCreate(
    TaskUS6
    ,  (const portCHAR *) "Ultrasonic6"
    ,  128  // Stack size
    ,  NULL
    ,  5  // Priority
    ,  NULL );

    
  xTaskCreate(
    TaskUS7
    ,  (const portCHAR *) "Ultrasonic7"
    ,  128  // Stack size
    ,  NULL
    ,  5  // Priority
    ,  NULL );

  xTaskCreate(
    TaskUS8
    ,  (const portCHAR *) "Ultrasonic8"
    ,  128  // Stack size
    ,  NULL
    ,  5  // Priority
    ,  NULL );
    
   for(int i = 0; i < 8; i++)
    {
      pinMode(led[i], OUTPUT);
    }
  
}

void loop()
{
  // Empty. Things are done in Tasks.
}

/*--------------------------------------------------*/
/*---------------------- Tasks ---------------------*/
/*--------------------------------------------------*/


/*00000000000000000000000000000000000000000000000000*/
/*-----------------ULTRASONIK 1--------------------*/
/*00000000000000000000000000000000000000000000000000*/


void TaskUS1(void *pvParameters)  // This is a task.
{
  (void) pvParameters;

  // initialize serial communication at 115200 bits per second
  Serial.begin(115200);
   for (;;)
  {
    vTaskDelay( 20 / portTICK_PERIOD_MS );
    int SRsensor = sonar[0].ping_cm();
    int pinled = led[0];
    if (SRsensor <= 15 && SRsensor != 0)
     {
        Serial.print("Ultra Sonik 1 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, HIGH);
     }
    if (SRsensor > 15)
     {
        Serial.print("Ultra Sonik 1 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, LOW); 
     }
   }
}


/*00000000000000000000000000000000000000000000000000*/
/*-----------------ULTRASONIK 2--------------------*/
/*00000000000000000000000000000000000000000000000000*/


void TaskUS2(void *pvParameters)  // This is a task.
{
  (void) pvParameters;

  // initialize serial communication at 115200 bits per second
  Serial.begin(115200);
 
  for (;;)
  {
    vTaskDelay( 20 / portTICK_PERIOD_MS );
    int SRsensor = sonar[1].ping_cm();
    int pinled = led[1];
    if (SRsensor <= 15 && SRsensor != 0)
     {
        Serial.print("Ultra Sonik 2 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, HIGH);
     }
    if (SRsensor > 15)
     {
        Serial.print("Ultra Sonik 2 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, LOW); 
     }
  }
}


/*00000000000000000000000000000000000000000000000000*/
/*-----------------ULTRASONIK 3--------------------*/
/*00000000000000000000000000000000000000000000000000*/



void TaskUS3(void *pvParameters)  // This is a task.
{
  (void) pvParameters;

  // initialize serial communication at 115200 bits per second
  Serial.begin(115200);
  
  for (;;)
  {
    vTaskDelay( 20 / portTICK_PERIOD_MS );
    int SRsensor = sonar[2].ping_cm();
    int pinled = led[2];
    if (SRsensor <= 15 && SRsensor != 0)
     {
        Serial.print("Ultra Sonik 3 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, HIGH);
     }
    if (SRsensor > 15)
     {
        Serial.print("Ultra Sonik 3 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, LOW); 
     }
  }
}



/*00000000000000000000000000000000000000000000000000*/
/*-----------------ULTRASONIK 4--------------------*/
/*00000000000000000000000000000000000000000000000000*/



void TaskUS4(void *pvParameters)  // This is a task.
{
  (void) pvParameters;

  // initialize serial communication at 115200 bits per second
  Serial.begin(115200);
  
  for (;;)
  {
    vTaskDelay( 20 / portTICK_PERIOD_MS );
    int SRsensor = sonar[3].ping_cm();
    int pinled = led[3];
    if (SRsensor <= 15 && SRsensor != 0)
     {
        Serial.print("Ultra Sonik 4 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, HIGH);
     }
    if (SRsensor > 15)
     {
        Serial.print("Ultra Sonik 4 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, LOW); 
     }
  }
}



/*00000000000000000000000000000000000000000000000000*/
/*-----------------ULTRASONIK 5--------------------*/
/*00000000000000000000000000000000000000000000000000*/



void TaskUS5(void *pvParameters)  // This is a task.
{
  (void) pvParameters;

  // initialize serial communication at 115200 bits per second
  Serial.begin(115200);
  
  for (;;)
  {
    vTaskDelay( 20 / portTICK_PERIOD_MS );
    int SRsensor = sonar[4].ping_cm();
    int pinled = led[4];
    if (SRsensor <= 15 && SRsensor != 0)
     {
        Serial.print("Ultra Sonik 5 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, HIGH);
     }
    if (SRsensor > 15)
     {
        Serial.print("Ultra Sonik 5 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, LOW); 
     }
  }
}



/*00000000000000000000000000000000000000000000000000*/
/*-----------------ULTRASONIK 6--------------------*/
/*00000000000000000000000000000000000000000000000000*/



void TaskUS6(void *pvParameters)  // This is a task.
{
  (void) pvParameters;

  // initialize serial communication at 115200 bits per second
  Serial.begin(115200);
  
  for (;;)
  {
    vTaskDelay( 20 / portTICK_PERIOD_MS );
    int SRsensor = sonar[5].ping_cm();
    int pinled = led[5];
    if (SRsensor <= 15 && SRsensor != 0)
     {
        Serial.print("Ultra Sonik 6 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, HIGH);
     }
    if (SRsensor > 15)
     {
        Serial.print("Ultra Sonik 6 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, LOW); 
     }
  }
}


/*00000000000000000000000000000000000000000000000000*/
/*-----------------ULTRASONIK 7--------------------*/
/*00000000000000000000000000000000000000000000000000*/


void TaskUS7(void *pvParameters)  // This is a task.
{
  (void) pvParameters;

  // initialize serial communication at 115200 bits per second
  Serial.begin(115200);
  
  for (;;)
  {
    vTaskDelay( 20 / portTICK_PERIOD_MS );
    int SRsensor = sonar[6].ping_cm();
    int pinled = led[6];
    if (SRsensor <= 15 && SRsensor != 0)
     {
        Serial.print("Ultra Sonik 7 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, HIGH);
     }
    if (SRsensor > 15)
     {
        Serial.print("Ultra Sonik 7 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, LOW); 
     }
  }
}



/*00000000000000000000000000000000000000000000000000*/
/*-----------------ULTRASONIK 8--------------------*/
/*00000000000000000000000000000000000000000000000000*/


void TaskUS8(void *pvParameters)  // This is a task.
{
  (void) pvParameters;

  // initialize serial communication at 115200 bits per second
  Serial.begin(115200);
 
  for (;;)
  {
     vTaskDelay( 20 / portTICK_PERIOD_MS );
    int SRsensor = sonar[7].ping_cm();
    int pinled = led[7];
    if (SRsensor <= 15 && SRsensor != 0)
     {
        Serial.print("Ultra Sonik 8 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, HIGH);
     }
    if (SRsensor > 15)
     {
        Serial.print("Ultra Sonik 8 : ");
        Serial.println(SRsensor);
        digitalWrite(pinled, LOW); 
     }

  }
}

