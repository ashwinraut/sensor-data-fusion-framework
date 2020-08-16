# sensor-data-fusion-framework

A framework to enable multi sensor fusion on Embedded devices.

The framework is intented to support multiple platforms , RTOS , Linux etc.

For use in small low power embedded devices like wearables to large embedded devices like Autonomous vehicles , Agricultural robots etc.

Framework will be able to support any kind of sensor stream for example:
Motion Sensors - Accel , Gyro , Mag
Light Sensors - Ambient light etc.
Health Sensors - PPG , ECG , Bio Impedance etc.
Autonomous Robots sensors - Camera , LiDar etc.
Weather sensors - UV sensors , Temperature sensor.

The goal is to provide a framework that can be used to interface any sensor and different kinds of algorithms DSP or ML.This is mainly achieved by converting the data into streams. The framework operates on the concept of streams, any sensor - virtual or physical or an algorithm can generate a stream or consume a stream.
This allows the user to create any kind of streams by writing an stream adapter or consume any stream using a stream adapter. Since the framework operates on the stream abstraction, it is possible to interface multiple different sensors, virtual sensor data recorders, replayers and algorithms, algorithms can also be chained to generate a derived stream.
The framework will reduce the efforts needed in writing the sensor data pipeline, data synchronization , data batching and data publishing and subscribing mechanisms.

The framework is designed to be used for interface DSP algorithms as well as the ML algorithms , in parallel or exclusively.
Eventually the goals is to create a repository of such algorithms that can be used by the users of the framework.

