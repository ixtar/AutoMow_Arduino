Arduino Uno Sketch to measure ultrasonic distance from three sensors and return through I2C to requesting devices

Continuosly polls three ultrasonic sensors:
1- Parallax PING ultrasonic sensor connected to pin 12
2- HC-SR04 ultrasonic sensor:
    trig - pin 2
    echo - pin 4
3- Parallax PING ultrasonic sensor connected to pin 5

Arduno has I2C address 0x11. Upon requrest, it will return an array of three bytes for each sensor like so [sensor_1_byte, sensor_2_byte, sensor_3_byte]
