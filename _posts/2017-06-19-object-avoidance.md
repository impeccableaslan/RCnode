---
ID: 505
post_title: Object avoidance
author: impeccableaslan
post_date: 2017-06-19 05:32:58
post_excerpt: ""
layout: post
permalink: >
  http://rcnode.com/index.php/2017/06/19/object-avoidance/
published: true
---
[et_pb_section fb_built="1" admin_label="section" _builder_version="3.0.47"][et_pb_row admin_label="row" _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4" _builder_version="3.0.47" parallax="off" parallax_method="on"][et_pb_text admin_label="Text" _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"]
					
				[/et_pb_text][et_pb_text _builder_version="3.0.51"]<h1>Obstacle detection (IR sensor)</h1>
<p>The IR sensors are used for obstacle detection .The sensor output signal send to the microcontroller. The microcontroller controls the vehicle (forward/back/stop) by using the DC motor which is placed in the vehicle. If any obstacle is placed in line the IR sensor fails to receive the light rays and gives signals to the microcontroller. The microcontroller will stop the vehicle immediately and siren will on. After one minute the robot will be check the path status, if obstacle is removed the robot move forward else the robot will return back to starting place. The sensor detects objects by emitting a short ultrasonic burst and then listening for the echo. Under control of a host microcontroller, the sensor emits a short 40 KHz explosion. This explosion ventures or travels through the air, hits an article and after that bounces once again to the sensor. The sensor provides an output pulse to the host that will terminate when the echo is detected; hence the width of one pulse to the next is taken into calculation by a program to provide result in distance of the object.</p>
<h1></h1>
<h1></h1>
<h1>Path detection (Proximity sensor)</h1>
<p>The normal case both sensors give the guidelines and robot follows it going straight on path. When the line end at that time the robot reverse at 180 and turns back the same place.[caption width="342" id="attachment_509" align="alignnone"]<img src="http://rcnode.com/wp-content/uploads/2017/06/path-detection.png" width="342" height="292" alt="" class="wp-image-509 size-full" /> Image from https://www.elprocus.com/obstacle-avoidance-robotic-vehicle/[/caption]</p>
<p>The proximity sensors are used for path detection. When the right sensor has not detect the curved line, the microcontroller activates the left motor to turn left until the right sensor receives a signal. Once signal is detected by the right sensor, the two motors are activated to go forward. When the line end at that time the robot reverse by 180 degrees and returns to starting position.</p>
<h1></h1>
<h1></h1>
<h1>Ultrasonic sensor</h1>
<p>These detects obstacles by emitting an ultrasonic wave and receiving it.[caption width="483" id="attachment_510" align="alignnone"]<img src="http://rcnode.com/wp-content/uploads/2017/06/ultrasonic-sensor.png" width="483" height="316" alt="" class="wp-image-510 size-full" /> Image from https://www.elprocus.com/obstacle-avoidance-robotic-vehicle/[/caption]</p>
<p>The ultrasonic sensor emits the short and high frequency signal. These propagate in the air at the velocity of sound. If they hit any object, then they reflect back echo signal to the sensor. The ultrasonic sensor consists of a multi vibrator, fixed to the base. The multi vibrator is combination of a resonator and vibrator. The resonator delivers ultrasonic wave generated by the vibration. The ultrasonic sensor actually consists of two parts; the emitter which produces a 40 kHz sound wave and detector detects 40 kHz sound wave and sends electrical signal back to the microcontroller.[caption width="475" id="attachment_511" align="alignnone"]<img src="http://rcnode.com/wp-content/uploads/2017/06/ultrasonic-sensor-2.png" width="475" height="187" alt="" class="wp-image-511 size-full" /> Image from https://www.elprocus.com/obstacle-avoidance-robotic-vehicle/[/caption]</p>
<p>When an electrical pulse of high voltage is applied to the ultrasonic transducer it vibrates across a specific spectrum of frequencies and generates a burst of sound waves. Whenever any obstacle comes ahead of the ultrasonic sensor the sound waves will reflect back in the form of echo and generates an electric pulse. It calculates the time taken between sending sound waves and receiving echo. The echo patterns will be compared with the patterns of sound waves to determine detected signal&rsquo;s condition.</p>
<h1></h1>
<h1></h1>
<h1>Analog vs digital</h1>
<p>Analog: Infinite</p>
<p>Digital: Finite&nbsp;</p>
<p>Signals are time-varying &ldquo;quantities&rdquo; which convey some sort of information. In electrical engineering the quantity that&rsquo;s time-varying is usually voltage (if not that, then usually current). So just think of them as a voltage that&rsquo;s changing over time. Signals are passed between devices in order to send and receive information, which might be video, audio, or some sort of encoded data. Usually the signals are transmitted through wires, but they could also pass through the air via radio frequency (RF) waves. Audio signals, for example might be transferred between your computer&rsquo;s audio card and speakers, while data signals might be passed through the air between a tablet and a WiFi router.</p>
<h1></h1>
<h1></h1>
<h1>Analog signals[caption width="605" id="attachment_512" align="alignnone"]<img src="http://rcnode.com/wp-content/uploads/2017/06/analog-signals.png" width="605" height="253" alt="" class="wp-image-512 size-full" /> Image from https://learn.sparkfun.com/tutorials/analog-vs-digital[/caption]</h1>
<p>A time versus voltage graph of an analog signal would be continuous and smooth. While these signals may be limited to a range of maximum and minimum values, there are still an infinite number of possible values within that range. For example, the analog voltage coming out of your wall socket might be clamped between -120V and +120V, but, as you increase the resolution more and more, you discover an infinite number of values that the signal can actually be (like 64.4V, 64.42V, 64.424V, and infinite, increasingly precise values).</p>
<h1></h1>
<h1></h1>
<h1>Digital signals</h1>
<p>Digital signals must have a finite set of possible values. The number of values in the set can be anywhere between two and a-very-large-number-that&rsquo;s-not-infinity. Most commonly digital signals will be one of two values &ndash; like either 0V or 5V. Timing graphs of these signals look like square waves.[caption width="605" id="attachment_513" align="alignnone"]<img src="http://rcnode.com/wp-content/uploads/2017/06/digital-signal.png" width="605" height="215" alt="" class="wp-image-513 size-full" /> Image from https://learn.sparkfun.com/tutorials/analog-vs-digital[/caption]</p>
<p>Or a digital signal might be a discrete representation of an analog waveform. Viewed from afar, the wave function below may seem smooth and analog, but when you look closely there are tiny discrete steps as the signal tries to approximate values:[caption width="605" id="attachment_514" align="alignnone"]<img src="http://rcnode.com/wp-content/uploads/2017/06/digital-signals-2.png" width="605" height="253" alt="" class="wp-image-514 size-full" /> Image from https://learn.sparkfun.com/tutorials/analog-vs-digital[/caption]</p>
<p>That&rsquo;s the big difference between analog and digital waves. Analog waves are smooth and continuous, digital waves are stepping, square, and discrete.</p>
<h1></h1>
<h1>Using ultrasonic sensors</h1>
<p>Microcontroller: is a self-contained system with peripherals, memory and a processor that can be used as an embedded system. Most programmable microcontrollers that are used today are embedded in other consumer products or machinery including phones, peripherals, automobiles and household appliances for computer systems. Due to that, another name for a microcontroller is "embedded controller." Some embedded systems are more sophisticated, while others have minimal requirements for memory and programming length and a low software complexity. Input and output devices include solenoids, LCD displays, relays, switches and sensors for data like humidity, temperature or light level, amongst others.</p>
<p>Control signal: A pulse or frequency of electricity or light that represents a control command as it travels over a network, a computer channel or wireless. In the data communications world, control signals typically travel the same path as the data either as separate packets or contained within the data packets. Think of control command as instructions sent to the processor.</p>
<p>&nbsp;Motor driver: A motor driver is a little current amplifier; the function of motor drivers is to take a low-current control signal and then turn it into a higher-current signal that can drive a motor.</p>
<p>&nbsp;GPIO pins: General-purpose input/output is a generic pin on an integrated circuit or computer board whose behavior&mdash;including whether it is an input or output pin&mdash;is controllable by the user at run time. These are used as it can both receive input and output.</p>
<p>&nbsp;Why use motor driver?: Without a motor driver, the microcontroller will burn out due to the high current passing through it. The solution is to use a motor driver. In addition, the microcontroller is not power enough to drive the motor, as it has GPIO pins. However, the motor drivers lack "the brain", thus they need the microcontroller to tell them what to do. These are not directly connected to the microcontroller and needs an alternative power source as they pull power from the power source. So if it's connected to the microcontroller the current will go through the controller and burn it.</p>
<p>In this context, the microcontroller is literally a "controller". Motors are connected to the microcontroller through motor drive IC (Integrated circuit). The ultrasonic sensor is attached in front of the drone. Whenever the drone is going on the desired path the ultrasonic sensor transmits the ultrasonic waves continuously from its sensor head. Whenever an obstacle comes ahead of it the ultrasonic waves are reflected back from an object and that information is passed to the microcontroller. The microcontroller controls the motors left, right, back, front, based on ultrasonic signals. In order to control the speed of each motor pulse width modulation is used (PWM).</p>
<p>Control circuitry: The drive's internal logic board contains a microprocessor and internal memory, and other structures and circuits that control what happens inside the drive. In many ways, this is like a small embedded PC within the hard disk itself</p>
<p>Pulse width modulation: PWM is a fancy term for describing a type of digital signal. Pulse width modulation is used in a variety of applications including sophisticated control circuitry. Pulse width modulation allows us to vary how much time the signal is high in an analog fashion. While the signal can only be high (usually 5V) or low (ground) at any time, we can change the proportion of time the signal is high compared to when it is low over a consistent time interval.[caption width="628" id="attachment_515" align="alignnone"]<img src="http://rcnode.com/wp-content/uploads/2017/06/waveform.png" width="628" height="356" alt="" class="wp-image-515 size-full" /> Image from https://learn.sparkfun.com/tutorials/pulse-width-modulation[/caption]</p>
<p>Waveform: A waveform is the shape and form of a signal such as a wave moving in a physical medium or an abstract representation.</p>
<h1></h1>
<h1>Duty cycle</h1>
<p>When the signal is high, we call this &ldquo;on time&rdquo;. To describe the amount of &ldquo;on time&rdquo; , we use the concept of duty cycle. Duty cycle is measured in percentage. The percentage duty cycle specifically describes the percentage of time a digital signal is on over an interval or period of time. This period is the inverse of the frequency of the waveform.[caption width="650" id="attachment_516" align="alignnone"]<img src="http://rcnode.com/wp-content/uploads/2017/06/duty-cycle.png" width="650" height="446" alt="" class="wp-image-516 size-full" /> Image from https://learn.sparkfun.com/tutorials/pulse-width-modulation[/caption]</p>
<p>If a digital signal spends half of the time on and the other half off, we would say the digital signal has a duty cycle of 50% and resembles an ideal square wave. If the percentage is higher than 50%, the digital signal spends more time in the high state than the low state and vice versa if the duty cycle is less than 50%.&nbsp; 100% duty cycle would be the same as setting the voltage to 5 Volts (high). 0% duty cycle would be the same as grounding the signal.&nbsp;</p>
<p>The pulse width modulation controls this duty cycle. It is a technique for getting analog results with digital means.</p>
<p>You can also use pulse width modulation to control the angle of a servo motor attached to something mechanical like a robot arm. Servos have a shaft that turns to specific position based on its control line. Our servo motors have a range of about 180 degrees. Frequency/period are specific to controlling a specific servo. A typical servo motor expects to be updated every 20 ms with a pulse between 1 ms and 2 ms, or in other words, between a 5 and 10% duty cycle on a 50 Hz waveform. With a 1.5 ms pulse, the servo motor will be at the natural 90 degree position. With a 1 ms pulse, the servo will be at the 0 degree position, and with a 2 ms pulse, the servo will be at 180 degrees. You can obtain the full range of motion by updating the servo with an value in between.</p>
<h1></h1>
<h1>Logic levels</h1>
<p>A logic level is a specific voltage or a state in which a signal can exist. We often refer to the two states in a digital circuit to be ON or OFF. Represented in binary, an ON translates to a binary 1, and an OFF translates to a binary 0. In Arduino, we call these signals HIGH or LOW, respectively. There are several different technologies that have evolved over the past 30 years in electronics to define the various voltage levels.</p>
<p>Logic 0 or Logic 1: Digital electronics rely on binary logic to store, process, and transmit data or information. Binary Logic refers to one of two states &ndash; ON or OFF. This is commonly translated as a binary 1 or binary 0. A binary 1 is also referred to as a HIGH signal and a binary 0 is referred to as a LOW signal. The strength of a signal is typically described by its voltage level. How is a logic 0 (LOW) or a logic 1 (HIGH) defined? Manufacturers of chips generally define these in their spec sheets. The most common standard is TTL or Transistor-Transistor Logic.</p>
<p>Active-Low and Active-High: When working with ICs and microcontrollers, you&rsquo;ll likely encounter pins that are active-low and pins that are active-high. Simply put, this just describes how the pin is activated. If it&rsquo;s an active-low pin, you must &ldquo;pull&rdquo; that pin LOW by connecting it to ground. For an active high pin, you connect it to your HIGH voltage (usually 3.3V/5V).</p>
<p>For example, let&rsquo;s say you have a shift register that has a chip enable pin, CE. If you see the CE pin anywhere in the datasheet with a line over it like this, CE, then that pin is active-low. The CE pin would need to be pulled to GND in order for the chip to become enabled. If, however, the CE pin doesn&rsquo;t have a line over it, then it is active high, and it needs to be pulled HIGH in order to enable the pin.</p>
<p>&nbsp;Many ICs will have both active-low and active-high pins intermingled. Just be sure to double check for pin names that have a line over them. The line is used to represent NOT (also known as bar). When something is NOTTED, it changes to the opposite state. So if an active-high input is NOTTED, then it is now active-low. Simple as that!</p>
<p>&nbsp;Bipolar transistors: Bipolar transistors work as current-controlled current regulators. In other words, transistors restrict the amount of current passed according to a smaller, controlling current.</p>
<h1></h1>
<h1>TTL Logic Levels</h1>
<p>A majority of systems we use rely on 5 V TTL Logic Levels. TTL is an acronym for Transistor-Transistor Logic. It relies on circuits built from bipolar transistors to achieve switching and maintain logic states. Transistors are basically fancy-speak for electrically controlled switches. For any logic family, there are a number of threshold voltage levels to know:</p>
<p>VOH &ndash; Minimum OUTPUT Voltage level a TTL device will provide for a HIGH signal.</p>
<p>VIH &ndash; Minimum INPUT Voltage level to be considered a HIGH.</p>
<p>VOL &ndash; Maximum OUTPUT Voltage level a device will provide for a LOW signal.</p>
<p>VIL &ndash; Maximum INPUT Voltage level to still be considered a LOW.[caption width="120" id="attachment_517" align="alignnone"]<img src="http://rcnode.com/wp-content/uploads/2017/06/TTL.png" width="120" height="400" alt="" class="wp-image-517 size-full" /> Image from https://learn.sparkfun.com/tutorials/logic-levels[/caption]</p>
<p>You will notice that the minimum output HIGH voltage (VOH) is 2.7 V. Basically, this means that output voltage of the device driving HIGH will always be at least 2.7 V. The minimum input HIGH voltage (VIH) is 2 V, or basically any voltage that is at least 2 V will be read in as a logic 1 (HIGH) to a TTL device. You will also notice that there is cushion of 0.7 V between the output of one device and the input of another. This is sometimes referred to as noise margin.</p>
<p>Noise margin: The amount by which a signal exceeds the minimum amount for proper operation.</p>
<p>What happens if you have a voltage that is in between 0.8 V and 2 V? Well, your guess is as good as mine. Honestly, this range of voltages is undefined and results in an invalid state, often referred to as floating. If an output pin on your device is &ldquo;floating&rdquo; in this range, there is no certainty with what the signal will result in. It may bounce arbitrarily between HIGH and LOW.</p>
<p>Footprint: The amount of space a particular unit of hardware or software occupies. So smaller footprint would mean occupying less space.</p>
<h1></h1>
<h1>3.3 V CMOS Logic Levels</h1>
<p>As technology has advanced, people have created devices that require lower power consumption and run off a lower base voltage (Vcc = 3.3 V instead of 5 V). The fabrication technique is also a bit different for 3.3 V devices that allows a smaller footprint and lower overall system costs.[caption width="230" id="attachment_518" align="alignnone"]<img src="http://rcnode.com/wp-content/uploads/2017/06/logic-families.png" width="230" height="427" alt="" class="wp-image-518 size-full" /> Image from https://learn.sparkfun.com/tutorials/logic-levels[/caption]</p>
<p>In order to ensure general compatibility, you will notice that most of the voltage levels are almost all the same as 5 V devices. A 3.3 V device can interface with a 5V device without any additional components. For example, a logic 1 (HIGH) from a 3.3 V device will be at least 2.4 V. This will still be interpreted as a logic 1 (HIGH) to a 5V system because it is above the VIH of 2 V.</p>
<p>Be careful when going the other direction and interfacing from a 5 V to a 3.3 V device and ensure that the 3.3 V device is 5 V tolerant. The specification you are interested in is the maximum input voltage. On certain 3.3 V devices, any voltages above 3.6 V will cause permanent damage to the chip. You can use a simple voltage divider (like a 1K&Omega; and a 2K&Omega;) to knock down 5 V signals to 3.3 V levels.[caption width="223" id="attachment_519" align="alignnone"]<img src="http://rcnode.com/wp-content/uploads/2017/06/atmega.png" width="223" height="627" alt="" class="wp-image-519 size-full" /> Image from https://learn.sparkfun.com/tutorials/logic-levels[/caption]</p>
<p>The Arduino is built on a slightly more robust platform. The most noticeable difference is that the invalid region of voltages is only between 1.5 V and 3.0 V. The noise margin is greater on the Arduino and it has a higher threshold for a LOW signal. This makes building interfaces and working with other hardware much simpler.</p>
<h1>LightWare SF40c for Object Avoidance</h1>
<p>Mounting the SF40c-[caption width="524" id="attachment_520" align="alignnone"]<img src="http://rcnode.com/wp-content/uploads/2017/06/SF40c.png" width="524" height="565" alt="" class="wp-image-520 size-full" /> Image from ardupilot.org[/caption]</p>
<p>The SF40c should be mounted on the top or bottom of the vehicle so that the rotating portion scans horizontally and its view is not obstructed by any portion of the vehicle including GPS mast, vehicle legs etc. The round gold and black lightware logo should be facing forward.</p>
<p></p>
<p>Connecting to the pixhawk:[caption width="956" id="attachment_521" align="alignnone"]<img src="http://rcnode.com/wp-content/uploads/2017/06/sf40c-pixhawk.png" width="956" height="601" alt="" class="wp-image-521 size-full" /> Image from ardupilot.org[/caption]</p>
<p>The diagram above shows how the SF40c can be connected to the flight controller&rsquo;s serial input. The above pictures shows use of Serial4 but any free serial port can be used.</p>
<p>To configure it: <a href="http://ardupilot.org/copter/docs/common-lightware-sf40c-objectavoidance.html">http://ardupilot.org/copter/docs/common-lightware-sf40c-objectavoidance.html</a></p>
<h1>TeraRanger Tower for Object Avoidance</h1>
<p>Mounting the Sensor-[caption width="640" id="attachment_524" align="alignnone"]<img src="http://rcnode.com/wp-content/uploads/2017/06/Teraranger.png" width="640" height="433" alt="" class="wp-image-524 size-full" /> Image for ardupilot.org[/caption]</p>
<p>The TeraRanger Tower should be mounted on the top of the vehicle so that sensors scans horizontally and its view is not obstructed by any portion of the vehicle including GPS mast, vehicle legs etc.</p>
<p>Configuration: http://ardupilot.org/copter/docs/common-teraranger-tower-objectavoidance.html</p>[/et_pb_text][et_pb_divider show_divider="on" _builder_version="3.0.51" color="#000000" divider_weight="2px"][/et_pb_divider][et_pb_comments _builder_version="3.0.51"][/et_pb_comments][/et_pb_column][/et_pb_row][/et_pb_section]