- 👋 Hi, I’m @Nschweifler1
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Nschweifler1/Nschweifler1 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
Format: 
Plat-xxxx = Crash suspected to be x 
Post segment of code. 


=========================================================================================== 

PLAT-5668 | Crash suspected to be: 


TV target string:
  [Error] ###API Socket Exception###java.net.SocketException: Software caused connection abortSoftware caused connection abort 
r.<computed> @ 2.b0c04c1e.chunk.js:2 
  [Error] ###Image Socket Exception###java.net.SocketException: Software caused connection abortSoftware caused connection abort 

Lenovo Tablet logs:
07-05 19:01:33.628 10128  3196  3661 W System.err: 	at com.mvihealth.sockethost.SocketRelayReplyThread.run(SocketRelayReplyThread.java:35) 
07-05 19:01:33.628 10128  3196  4188 W System.err: java.net.SocketException: Software caused connection abort 
07-05 19:01:33.628 10128  3196  3661 E LogMessage (level Error): ###API Socket Exception### 
07-05 19:01:33.628 10128  3196  3661 E LogMessage (level Error): java.net.SocketException: Software caused connection abort 
07-05 19:01:33.628 10128  3196  3661 E LogMessage (level Error): Software caused connection abort 
07-05 19:01:33.628 10128  3196  4188 W System.err: 	at java.net.SocketInputStream.socketRead0(Native Method) 
07-05 19:01:33.628 10128  3196  4188 W System.err: 	at java.net.SocketInputStream.socketRead(SocketInputStream.java:119) 
07-05 19:01:33.628 10128  3196  4188 W System.err: 	at java.net.SocketInputStream.read(SocketInputStream.java:176) 
07-05 19:01:33.628 10128  3196  4188 W System.err: 	at java.net.SocketInputStream.read(SocketInputStream.java:144) 
07-05 19:01:33.628 10128  3196  4188 W System.err: 	at java.io.DataInputStream.readFully(DataInputStream.java:198) 
07-05 19:01:33.629 10128  3196  4188 W System.err: 	at java.io.DataInputStream.readShort(DataInputStream.java:317) 
07-05 19:01:33.629 10128  3196  4188 W System.err: 	at com.mvihealth.sockethost.SocketImageReplyThread.run(SocketImageReplyThread.java:51) 
07-05 19:01:33.629 10128  3196  4188 E LogMessage (level Error): ###Image Socket Exception### 
07-05 19:01:33.629 10128  3196  4188 E LogMessage (level Error): java.net.SocketException: Software caused connection abort 
07-05 19:01:33.629 10128  3196  4188 E LogMessage (level Error): Software caused connection abort 
07-05 19:01:33.629 10128  3196  3661 E LogMessage (level System): Closing data connectionSocket[address=/10.220.8.100,port=44438,localPort=8082] 
07-05 19:01:33.629 10128  3196  4188 E LogMessage (level System): Closing image connectionSocket[address=/10.220.8.100,port=53258,localPort=8080] 
07-05 19:01:33.639  root   748   946 D CommandListener: Clearing all IP addresses on wlan0 

HTC HMD logs:
<6>[    4.397637] c7    861 CAM_ERR: CAM-SENSOR: cam_sensor_core_power_up: 2037 usr_idx:100 dts_idx:3 
<6>[    4.399517] c6   1185 subsys-pil-tz aab0000.qcom,venus: venus: Brought out of reset 
<6>[    4.399740] c4    861 qcom,camera ac4f000.qcom,cci:qcom,cam-sensor4: Linked as a consumer to regulator.53 
<3>[    4.400079] c4    333 cnss: Antenna switch request failed, result: 1, err: 94 
<7>[    4.400085] c4    333 cnss: Sending mode message, mode: CALIBRATION(7), state: 0xf 
<6>[    4.402244] c5    861 qcom,camera ac4f000.qcom,cci:qcom,cam-sensor4: Linked as a consumer to regulator.37 
<6>[    4.402598] c5    861 qcom,camera ac4f000.qcom,cci:qcom,cam-sensor4: Linked as a consumer to regulator.81 
<6>[    4.411298] c6   1185 msm_vidc:   high: 00000001: ....d: Closed video instance: 0000000000000000 
<6>[    4.411331] c6   1185 msm_vidc:   high: 00000001: ....e: Opening video instance: 0000000000000000, 0 
<6>[    4.411396] c6   1185 msm_vidc:   high: 00000001: ....e: Closed video instance: 0000000000000000 
<6>[    4.424289] c4    861 CAM_INFO: CAM-SENSOR: cam_sensor_driver_cmd: 798 Probe success,slot:4,slave_addr:0xc0,sensor_id:0x9281 
<6>[    4.424344] c4    861 qcom,camera ac4f000.qcom,cci:qcom,cam-sensor4: Dropping the link to regulator.81 
<6>[    4.428098] c4    861 qcom,camera ac4f000.qcom,cci:qcom,cam-sensor4: Dropping the link to regulator.37 
<6>[    4.428145] c4    861 qcom,camera ac4f000.qcom,cci:qcom,cam-sensor4: Dropping the link to regulator.53 
<6>[    4.428150] c4    861 CAM_ERR: CAM-SENSOR: cam_sensor_util_power_down: 2320 seq_val:100 > num_vreg: 3 

TV > Tablet > HMD  compared for the same event with the same time frame when compared. 

=========================================================================================== 

PLAT-5656 | Crash Suspected to be: 

TV Target String:
"id":"2f01280a-85c3-bdf0-998f-3529-1656710005083","data":["%c [System] Closing image connectionSocket[address=/10.220.8.102,port=34654,localPort=8080]","color:  #008844"], 
"timestamp":"07-01 21:13:24.497"},{"method":"error","id":"a73edee9-96b3-c335-6818-1361-1656710005085", 
"data":["%c [Error] ###API Socket Exception###java.net.SocketException: Connection resetConnection reset", 
"color:  #008844"],"timestamp":"07-01 21:13:24.500"},{"method":"warn","id":"4c4f28b5-43de-09d6-d5bd-9842-1656710005088", 
"data":["%c [System] Closing data connectionSocket[address=/10.220.8.102,port=41338,localPort=8082]","color:  #008844"], 
"timestamp":"07-01 21:13:24.502"},{"method":"error","id":"8a051e38-817d-cb37-447f-9b1e-1656710007331", 
"data":["%c [Error] ###Error Sending Message to Tablet###java.net.SocketException: Socket closedSocket closed","color:  #008844"], 
"timestamp":"07-01 21:13:26.746"},{"method":"info","id":"02e37167-4ddf-83f2-2678-e0ec-1656710008224","data":[{"type":"Sensors_ResetCalibration","recalibrate":false}], 
"timestamp":"07-01 21:13:27.639"},{"method":"info","id":"998067a0-5b47-e486-7e47-3016-1656710009304","data" 

Lenovo Tablet Logs:
07-01 17:13:25.007 10143  7042  7250 E LogMessage (level Error): ###Image Socket Exception### 
07-01 17:13:25.007 10143  7042  7250 E LogMessage (level Error): java.io.EOFException 
07-01 17:13:25.007 10143  7042  7250 E LogMessage (level Error): null 
07-01 17:13:25.008 10143  7042  7250 E LogMessage (level System): Closing image connectionSocket[address=/10.220.8.102,port=34654,localPort=8080] 
07-01 17:13:25.019 10097  7251  7339 D OlmAppSessionManager: AppFirstActivityPostResumed event handlers 
07-01 17:13:25.021 10097  7251  7339 D HxServices: No hx accounts, not checking settings 
07-01 17:13:25.024 10143  7042  7165 W System.err: java.net.SocketException: Connection reset 
07-01 17:13:25.024 10143  7042  7165 W System.err: 	at java.net.SocketInputStream.read(SocketInputStream.java:215) 
07-01 17:13:25.025 10143  7042  7165 W System.err: 	at java.net.SocketInputStream.read(SocketInputStream.java:144) 
07-01 17:13:25.025 10143  7042  7165 W System.err: 	at java.io.DataInputStream.readFully(DataInputStream.java:198) 
07-01 17:13:25.025 10143  7042  7165 W System.err: 	at java.io.DataInputStream.readShort(DataInputStream.java:317) 
07-01 17:13:25.025 10143  7042  7165 W System.err: 	at com.mvihealth.sockethost.SocketRelayReplyThread.run(SocketRelayReplyThread.java:35) 
07-01 17:13:25.025 10143  7042  7165 E LogMessage (level Error): ###API Socket Exception### 
07-01 17:13:25.025 10143  7042  7165 E LogMessage (level Error): java.net.SocketException: Connection reset 
07-01 17:13:25.025 10143  7042  7165 E LogMessage (level Error): Connection reset 
07-01 17:13:25.026 10143  7042  7165 E LogMessage (level System): Closing data connectionSocket[address=/10.220.8.102,port=41338,localPort=8082] 
07-01 17:13:25.055 10097  7251  7339 D HxPushNotificationsManager: Hx FCM Token is-empty false is-different false . If empty or different, job to update will be kicked 
07-01 17:13:25.088 10097  7251  7339 W AveryInitialization: Avery###: AveryInitialization constructor being called: 
07-01 17:13:25.088 10097  7251  7339 W AveryInitialization:  
07-01 17:13:25.088 10097  7251  7339 W AveryInitialization:   com.avery.Avery@a277050 
07-01 17:13:25.088 10097  7251  7339 W AveryInitialization:    
07-01 17:13:25.115 10013 30080 30080 D BoundBrokerSvc: onUnbind: Intent { act=com.google.android.gms.measurement.START pkg=com.google.android.gms } 
07-01 17:13:25.643  1000   571   571 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0 
07-01 17:13:27.148  1000   571   571 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0 
07-01 17:13:27.319 10143  7042  7126 W System.err: java.net.SocketException: Socket closed 
07-01 17:13:27.319 10143  7042  7126 W System.err: 	at java.net.SocketOutputStream.socketWrite(SocketOutputStream.java:124) 
07-01 17:13:27.319 10143  7042  7126 W System.err: 	at java.net.SocketOutputStream.write(SocketOutputStream.java:140) 
07-01 17:13:27.319 10143  7042  7126 W System.err: 	at java.io.DataOutputStream.writeShort(DataOutputStream.java:167) 
07-01 17:13:27.320 10143  7042  7126 W System.err: 	at com.mvihealth.sockethost.RawSocketRelayThread.relayMessageFromTablet(RawSocketRelayThread.java:30) 
07-01 17:13:27.320 10143  7042  7126 W System.err: 	at com.penumbrainc.mvihealth.tablet.test.MainActivity.MessageReceived(MainActivity.java:392) 
07-01 17:13:27.320 10143  7042  7126 W System.err: 	at com.mvihealth.sockethost.OurWebSocketServer.onMessage(OurWebSocketServer.java:103) 
07-01 17:13:27.320 10143  7042  7126 W System.err: 	at org.java_websocket.server.WebSocketServer.onWebsocketMessage(WebSocketServer.java:703) 
07-01 17:13:27.320 10143  7042  7126 W System.err: 	at org.java_websocket.drafts.Draft_6455.processFrameText(Draft_6455.java:963) 
07-01 17:13:27.320 10143  7042  7126 W System.err: 	at org.java_websocket.drafts.Draft_6455.processFrame(Draft_6455.java:887) 
07-01 17:13:27.320 10143  7042  7126 W System.err: 	at org.java_websocket.WebSocketImpl.decodeFrames(WebSocketImpl.java:401) 
07-01 17:13:27.320 10143  7042  7126 W System.err: 	at org.java_websocket.WebSocketImpl.decode(WebSocketImpl.java:233) 
07-01 17:13:27.320 10143  7042  7126 W System.err: 	at org.java_websocket.server.WebSocketServer$WebSocketWorker.doDecode(WebSocketServer.java:1096) 
07-01 17:13:27.321 10143  7042  7126 W System.err: 	at org.java_websocket.server.WebSocketServer$WebSocketWorker.run(WebSocketServer.java:1077) 
07-01 17:13:27.321 10143  7042  7126 E LogMessage (level Error): ###Error Sending Message to Tablet### 
07-01 17:13:27.321 10143  7042  7126 E LogMessage (level Error): java.net.SocketException: Socket closed 
07-01 17:13:27.321 10143  7042  7126 E LogMessage (level Error): Socket closed 
07-01 17:13:27.322 10143  7042  7126 I System.out: org.java_websocket.WebSocketImpl@5792902: {"Ping":"2022-07-01T21:13:27.315Z"} 
07-01 17:13:27.395  1000   571   571 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0 
07-01 17:13:33.394  1000   571   571 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0 
07-01 17:13:33.549 10143  7042  7126 I System.out: org.java_websocket.WebSocketImpl@5792902: {"Ping":"2022-07-01T21:13:33.545Z"} 
07-01 17:13:34.311  root   754   871 E storaged: getDiskStats failed with result NOT_SUPPORTED and size 0 
07-01 17:13:38.308 10143  7042  7042 I AssistStructure: Flattened final assist data: 3508 bytes, containing 1 windows, 7 views 

HTC HMD Logs:
<14>[  323.997626] c3      1 init: Received control message 'start' for 'dumpstatez' from pid: 4233 (bugreportz -p) 
<14>[  323.998133] c3      1 init: starting service 'dumpstatez'... 
<14>[  324.000223] c0   4235 init: Created socket '/dev/socket/dumpstate', mode 660, user 2000, group 1007 
<14>[  325.127585] c3      1 init: Received control message 'interface_start' for 'android.hardware.biometrics.fingerprint@2.1::IBiometricsFingerprint/default' from pid: 569 (/system/bin/hwservicemanager) 
<11>[  325.127637] c3      1 init: Could not find 'android.hardware.biometrics.fingerprint@2.1::IBiometricsFingerprint/default' for ctl.interface_start 
<36>[  325.238998] c0    586 type=1400 audit(1656710167.755:1818): avc: granted { read } for comm="main" name="u:object_r:net_dns_prop:s0" dev="tmpfs" ino=22045 scontext=u:r:untrusted_app_25:s0:c512,c768 tcontext=u:object_r:net_dns_prop:s0 tclass=file 
<38>[  325.239019] c0    586 type=1400 audit(1656710172.339:1819): avc: denied { ptrace } for comm="crash_dump64" scontext=u:r:crash_dump:s0 tcontext=u:r:vold:s0 tclass=process permissive=1 
<14>[  325.269804] c3      1 init: Untracked pid 4254 exited with status 0 
<14>[  325.270605] c3      1 init: Untracked pid 4256 exited with status 0 
<14>[  325.352180] c3      1 init: Untracked pid 4260 exited with status 0 
<14>[  325.353302] c3      1 init: Untracked pid 4262 exited with status 0 
<14>[  325.581689] c3      1 init: Untracked pid 4265 exited with status 0 
<14>[  325.586715] c3      1 init: Untracked pid 4267 exited with status 0 
<14>[  325.619865] c3      1 init: Untracked pid 4270 exited with status 0 
<14>[  325.620328] c3      1 init: Untracked pid 4272 exited with status 0 
<14>[  325.659590] c3      1 init: Untracked pid 4275 exited with status 0 
<14>[  325.659661] c3      1 init: Untracked pid 4277 exited with status 0 
<14>[  325.752377] c3      1 init: Untracked pid 4280 exited with status 0 
<14>[  325.763917] c3      1 init: Untracked pid 4282 exited with status 0 
<14>[  325.775963] c3      1 init: Untracked pid 4286 exited with status 0 
<14>[  325.777070] c3      1 init: Untracked pid 4288 exited with status 0 
<14>[  325.805991] c3      1 init: Untracked pid 4292 exited with status 0 
<14>[  325.806742] c3      1 init: Untracked pid 4294 exited with status 0 
<14>[  325.844550] c3      1 init: Untracked pid 4298 exited with status 0 
<14>[  325.845280] c3      1 init: Untracked pid 4300 exited with status 0 
<14>[  325.874275] c3      1 init: Untracked pid 4305 exited with status 0 
<14>[  325.874357] c3      1 init: Untracked pid 4303 exited with status 0 
<14>[  325.908748] c3      1 init: Untracked pid 4308 exited with status 0 
<14>[  325.909215] c3      1 init: Untracked pid 4310 exited with status 0 
<14>[  325.981514] c3      1 init: Untracked pid 4314 exited with status 0 
<14>[  325.986969] c3      1 init: Untracked pid 4316 exited with status 0 
<14>[  326.050027] c3      1 init: Untracked pid 4320 exited with status 0 
<14>[  326.056923] c3      1 init: Untracked pid 4322 exited with status 0 
<14>[  326.125478] c3      1 init: Untracked pid 4325 exited with status 0 
<14>[  326.128096] c3      1 init: Untracked pid 4327 exited with status 0 
<14>[  326.372231] c3      1 init: Untracked pid 4330 exited with status 0 
<14>[  326.374809] c3      1 init: Untracked pid 4332 exited with status 0 
<14>[  326.580356] c3      1 init: Untracked pid 4336 exited with status 0 
<14>[  326.582418] c3      1 init: Untracked pid 4338 exited with status 0 
<14>[  326.626142] c3      1 init: Untracked pid 4342 exited with status 0 
<14>[  326.627164] c3      1 init: Untracked pid 4344 exited with status 0 
<14>[  326.696770] c3      1 init: Untracked pid 4348 exited with status 0 
<14>[  326.699542] c3      1 init: Untracked pid 4350 exited with status 0 
<14>[  326.913155] c3      1 init: Untracked pid 4353 exited with status 0 
<14>[  326.915227] c3      1 init: Untracked pid 4355 exited with status 0 
<14>[  326.965277] c3      1 init: Untracked pid 4359 exited with status 0 
<14>[  326.966342] c3      1 init: Untracked pid 4361 exited with status 0 
<14>[  327.053735] c3      1 init: Untracked pid 4365 exited with status 0 
<14>[  327.055153] c3      1 init: Untracked pid 4367 exited with status 0 
  
=========================================================================================== 

PLAT-5647 | Crash Suspected to be: 
[First Set of logs from Max] 


TV Target String:
Exception found on line 15915 in [ 7943 : AndroidRuntime ]: FATAL EXCEPTION: socketImageReplyThread_count10 
AndroidRuntime: Process: com.penumbrainc.mvihealth.tablet.test, PID: 7943 
AndroidRuntime: java.lang.NullPointerException: Attempt to invoke virtual method 'java.lang.Object android.content.Context.getSystemService(java.lang.String)' on a null object reference 
AndroidRuntime: at com.penumbrainc.mvihealth.tablet.test.MainActivity.getAvailableMemory(MainActivity.java:533) 
AndroidRuntime: at com.penumbrainc.mvihealth.tablet.test.MainActivity.LowMemory(MainActivity.java:519) 
AndroidRuntime: at com.mvihealth.sockethost.SocketImageReplyThread.run(SocketImageReplyThread.java:75)  
Exception found on line 15917 in [ 7943 : AndroidRuntime ]: java.lang.NullPointerException: Attempt to invoke virtual method 'java.lang.Object android.content.Context.getSystemService(java.lang.String)' on a null object reference 
AndroidRuntime: at com.penumbrainc.mvihealth.tablet.test.MainActivity.getAvailableMemory(MainActivity.java:533) AndroidRuntime: at com.penumbrainc.mvihealth.tablet.test.MainActivity.LowMemory(MainActivity.java:519) 
AndroidRuntime: at com.mvihealth.sockethost.SocketImageReplyThread.run(SocketImageReplyThread.java:75)  
Exception found on line 20699 in [ 1376 : Ringtone ]: Remote playback not allowed: java.io.IOException: setDataSource failed. 
Ringtone: Problem opening; delegating to remote player 
Ringtone: Neither local nor remote player available when applying playback properties 
Ringtone: Neither local nor remote player available when applying playback properties  
Exception found on line 21256 in [ 6387 : Utility ]: android.content.pm.PackageManager$NameNotFoundException: com.lenovo.lsf.user  
Exception found on line 21413 in [ 6387 : Utility ]: android.content.pm.PackageManager$NameNotFoundException: com.lenovo.lsf.user 
SSOSingleUserAuth: getStatus offline 
Utility: android.content.pm.PackageManager$NameNotFoundException: com.lenovo.lsf.user 
SSOSingleUserAuth: getStatus offline 
BatteryInfo: time for callback: 0ms  
Exception found on line 21415 in [ 6387 : Utility ]: android.content.pm.PackageManager$NameNotFoundException: com.lenovo.lsf.user 
SSOSingleUserAuth: getStatus offline 
BatteryInfo: time for callback: 0ms  

Lenovo Tablet Logs:
06-24 14:31:09.750 10121  7943  9804 E AndroidRuntime: FATAL EXCEPTION: socketImageReplyThread_count10 
06-24 14:31:09.750 10121  7943  9804 E AndroidRuntime: Process: com.penumbrainc.mvihealth.tablet.test, PID: 7943 
06-24 14:31:09.750 10121  7943  9804 E AndroidRuntime: java.lang.NullPointerException: Attempt to invoke virtual method 'java.lang.Object android.content.Context.getSystemService(java.lang.String)' on a null object reference 
06-24 14:31:09.750 10121  7943  9804 E AndroidRuntime: 	at com.penumbrainc.mvihealth.tablet.test.MainActivity.getAvailableMemory(MainActivity.java:533) 
06-24 14:31:09.750 10121  7943  9804 E AndroidRuntime: 	at com.penumbrainc.mvihealth.tablet.test.MainActivity.LowMemory(MainActivity.java:519) 
06-24 14:31:09.750 10121  7943  9804 E AndroidRuntime: 	at com.mvihealth.sockethost.SocketImageReplyThread.run(SocketImageReplyThread.java:75) 

HTC HMD Logs:
This happened a few milli seconds later on the HMD -

<11>[    3.372662] c7      1 init: Could not start service 'esepmdaemon' as part of class 'core': Cannot find '/system/vendor/bin/esepmdaemon': No such file or directory 
<14>[    3.372739] c7      1 init: starting service 'vendor.lowi'... 
<14>[    3.373325] c7      1 init: starting service 'vendor.pd_mapper'... 
<14>[    3.373906] c7      1 init: starting service 'vendor.per_mgr'... 
<14>[    3.374543] c7      1 init: starting service 'vendor.mdm_launcher'... 
<14>[    3.375156] c7      1 init: starting service 'ashmemd'... 
<14>[    3.375820] c7      1 init: starting service 'audioserver'... 
<12>[    3.381993] c2    870 healthd: Unknown power supply type 'BMS' 
<12>[    3.382075] c2    870 healthd: Unknown power supply type 'Main' 
<14>[    3.388493] c4      1 init: starting service 'gpu'... 
<12>[    3.389257] c2    870 healthd: battery l=100 v=4254 t=28.7 h=2 st=3 c=-1013 fc=3944000 cc=17 chg= 
<14>[    3.389886] c4      1 init: starting service 'lmkd'... 
<14>[    3.390727] c4      1 init: starting service 'surfaceflinger'... 
<14>[    3.391732] c4      1 init: starting service 'vendor.rmt_storage'... 
<14>[    3.392576] c4      1 init: starting service 'vendor.tftp_server'... 
<38>[    3.398909] c5    582 type=1400 audit(1656624470.752:393): avc: denied { create } for comm="init" name="cp_interval" scontext=u:r:init:s0 tcontext=u:object_r:sysfs_fs_f2fs:s0 tclass=file permissive=1 
<38>[    3.398918] c5    582 type=1400 audit(1656624470.824:394): avc: denied { read } for comm="vendor.qti.hard" name="u:object_r:vendor_cap_configstore_dbg_prop:s0" dev="tmpfs" ino=24765 scontext=u:r:hal_capabilityconfigstore_qti_default:s0 tcontext=u:object_r:vendor_cap_configstore_dbg_prop:s0 tclass=file permissive=1 
<38>[    3.398959] c5    582 type=1400 audit(1656624470.824:394): avc: denied { read } for comm="vendor.qti.hard" name="u:object_r:vendor_cap_configstore_dbg_prop:s0" dev="tmpfs" ino=24765 scontext=u:r:hal_capabilityconfigstore_qti_default:s0 tcontext=u:object_r:vendor_cap_configstore_dbg_prop:s0 tclass=file permissive=1 
<38>[    3.398963] c5    582 type=1400 audit(1656624470.824:395): avc: denied { open } for comm="vendor.qti.hard" path="/dev/__properties__/u:object_r:vendor_cap_configstore_dbg_prop:s0" dev="tmpfs" ino=24765 scontext=u:r:hal_capabilityconfigstore_qti_default:s0 tcontext=u:object_r:vendor_cap_configstore_dbg_prop:s0 tclass=file permissive=1 
<38>[    3.398978] c5    582 type=1400 audit(1656624470.824:395): avc: denied { open } for comm="vendor.qti.hard" path="/dev/__properties__/u:object_r:vendor_cap_configstore_dbg_prop:s0" dev="tmpfs" ino=24765 scontext=u:r:hal_capabilityconfigstore_qti_default:s0 tcontext=u:object_r:vendor_cap_configstore_dbg_prop:s0 tclass=file permissive=1 
<38>[    3.398981] c5    582 type=1400 audit(1656624470.824:396): avc: denied { getattr } for comm="vendor.qti.hard" path="/dev/__properties__/u:object_r:vendor_cap_configstore_dbg_prop:s0" dev="tmpfs" ino=24765 scontext=u:r:hal_capabilityconfigstore_qti_default:s0 tcontext=u:object_r:vendor_cap_configstore_dbg_prop:s0 tclass=file permissive=1 
<38>[    3.398994] c5    582 type=1400 audit(1656624470.824:396): avc: denied { getattr } for comm="vendor.qti.hard" path="/dev/__properties__/u:object_r:vendor_cap_configstore_dbg_prop:s0" dev="tmpfs" ino=24765 scontext=u:r:hal_capabilityconfigstore_qti_default:s0 tcontext=u:object_r:vendor_cap_configstore_dbg_prop:s0 tclass=file permissive=1 
<38>[    3.398997] c5    582 type=1400 audit(1656624470.824:397): avc: denied { map } for comm="vendor.qti.hard" path="/dev/__properties__/u:object_r:vendor_cap_configstore_dbg_prop:s0" dev="tmpfs" ino=24765 scontext=u:r:hal_capabilityconfigstore_qti_default:s0 tcontext=u:object_r:vendor_cap_configstore_dbg_prop:s0 tclass=file permissive=1 
<14>[    3.401570] c4      1 init: Service 'irsc_util' (pid 905) exited with status 0
<14>[    3.401627] c4      1 init: processing action (boot) from (/init.rc:893) 
<14>[    3.401740] c4      1 init: starting service 'mlogger'... 
<14>[    3.402511] c4      1 init: processing action (boot) from (/init.usb.rc:21) 
<14>[    3.404641] c4    917 init: Created socket '/dev/socket/lmkd', mode 660, user 1000, group 1000 
<11>[    3.405105] c4    918 init: Failed to bind socket 'pdx/system/vr/display/client': No such file or directory 
<11>[    3.405238] c4    918 init: Failed to bind socket 'pdx/system/vr/display/manager': No such file or directory 
<11>[    3.405359] c4    918 init: Failed to bind socket 'pdx/system/vr/display/vsync': No such file or directory 
<14>[    3.405602] c4      1 init: processing action (persist.sys.usb.config=* && boot) from (/init.usb.rc:128) 
<14>[    3.405666] c4      1 init: processing action (boot) from (/vendor/etc/init/hw/init.htc_mia2.rc:10) 
<14>[    3.405873] c4      1 init: processing action (boot) from (/vendor/etc/init/hw/init.qcom.rc:110) 
<14>[    3.427014] c4    926 init: Created socket '/dev/socket/mld', mode 660, user 1000, group 1000 
<14>[    3.427199] c6      1 init: Command 'chmod 0755 /system/bin/ip' action=boot (/vendor/etc/init/hw/init.qcom.rc:166) took 0ms and failed: fchmodat() failed: Read-only file system 
<11>[    3.434434] c4    920 rmt_storage:ERR:main: Mmap Failed for rmts...pausing execution! 
<14>[    3.438637] c7      1 init: processing action (boot) from (/vendor/etc/init/hw/init.qcom.usb.rc:51) 
<14>[    3.438860] c7      1 init: Command 'mount configfs none /config' action=boot (/vendor/etc/init/hw/init.qcom.usb.rc:53) took 0ms and failed: mount() failed: Device or resource busy 

  
<<<<<<<<<<<<<<<<<>>>>>>>>>>>>>>>>>>>>> 

[Second Set of logs from Lynn] 
  
TV Target String:
2.b0c04c1e.chunk.js:2 TBL18 <<< 794ms {"FirmwareVersionNumber":"4.08.608.1","HMDSerialNumber":"FA0A52N00264"} 
2.b0c04c1e.chunk.js:2  apollo mutation upsert_device_and_firmwares (in 3 ms) 
2.b0c04c1e.chunk.js:2  apollo mutation updateUserSessionWithDeviceInfo (in 2 ms) 
2.b0c04c1e.chunk.js:2 HMD0020 <<< {"Command":"SystemEvent","Args":{"Event":"HeadsetOff"}} 
2.b0c04c1e.chunk.js:2  [Error] ###Image Socket Timeout Exception###Read timed out
r.<computed> @ 2.b0c04c1e.chunk.js:2 
2.b0c04c1e.chunk.js:2  [System] Closing image connectionSocket[address=/10.220.8.102,port=41158,localPort=8080] 
r.<computed> @ 2.b0c04c1e.chunk.js:2 
2.b0c04c1e.chunk.js:2 onDeviceKey volumeDown 1 
2.b0c04c1e.chunk.js:2 onDeviceKey volumeDown 0 
2.b0c04c1e.chunk.js:2 HMD disconnected 
2.b0c04c1e.chunk.js:2 [SENSORS]cancel sensorWorkflowSaga  
2.b0c04c1e.chunk.js:2 [SENSORS]finally sensorWorkflowSaga 
2.b0c04c1e.chunk.js:2  [Error] ###API Socket Exception###java.net.SocketException: Connection timed outConnection timed out 
r.<computed> @ 2.b0c04c1e.chunk.js:2 
2.b0c04c1e.chunk.js:2  [System] Closing data connectionSocket[address=/10.220.8.102,port=42176,localPort=8082] 
r.<computed> @ 2.b0c04c1e.chunk.js:2 
service-worker.js:28 Workbox is loaded 
2.b0c04c1e.chunk.js:2  [Error] ###Error Sending Message to Tablet###java.net.SocketException: Socket closedSocket closed 

Lenovo Tablet Logs:
07-01 17:22:35.738 10079  8696  8811 I LogMessage (level Message): raw socket string message:  
07-01 17:22:35.738 10079  8696  8811 I LogMessage (level Message): {"Pong":"2022-07-02T00:22:37.248Z"} 
07-01 17:22:36.379  root   551   597 E ANDR-PERF-MPCTL: Invalid profile no. 0, total profiles 0 only 
07-01 17:22:41.385  root   551   597 E ANDR-PERF-MPCTL: Invalid profile no. 0, total profiles 0 only 
07-01 17:22:41.765 10079  8696  8779 I System.out: org.java_websocket.WebSocketImpl@35de4d2: {"Ping":"2022-07-02T00:22:41.759Z"} 
07-01 17:22:43.275 10079  8696  8810 E LogMessage (level Error): ###Image Socket Timeout Exception### 
07-01 17:22:43.275 10079  8696  8810 E LogMessage (level Error): Read timed out 
07-01 17:22:43.277 10079  8696  8810 E LogMessage (level System): Closing image connectionSocket[address=/10.220.8.102,port=41158,localPort=8080] 
07-01 17:22:46.394  root   551   597 E ANDR-PERF-MPCTL: Invalid profile no. 0, total profiles 0 only 

HTC HMD Logs:







=========================================================================================== 

PLAT-5617 | Crash Suspected to be:

TV Target String:
4.c3380360.chunk.js:sourcemap:1149 LOGIN_SUCCESS
4.c3380360.chunk.js:sourcemap:1149 LOGGED_IN_AND_CONNECTED
2.55c473cc.chunk.js:sourcemap:2 TBL2 >>> {"Query":"SystemUpdateInfo"}
4.c3380360.chunk.js:sourcemap:1149 SET_SETTINGS
2.55c473cc.chunk.js:sourcemap:2 SET_RULES
2.55c473cc.chunk.js:sourcemap:2  apollo query facilityPatientSelectWithVisibility (in 4 ms)
2.55c473cc.chunk.js:sourcemap:2 > INIT Object
2.55c473cc.chunk.js:sourcemap:2 > RESULT Object
2.55c473cc.chunk.js:sourcemap:2 GAME_DISCONNECTED
2.55c473cc.chunk.js:sourcemap:2 HMD disconnected
4.c3380360.chunk.js:sourcemap:1149 LOGGED_IN_AND_CONNECTED
2.55c473cc.chunk.js:sourcemap:2 API timeout TBL1-4afd97e3-e695-48dc-a19d-9195c05efa9d Object
4.c3380360.chunk.js:sourcemap:1149 RETRYING_GAME_CONNECTION
2.55c473cc.chunk.js:sourcemap:2 TBL1 >>> {"Query":"Version"}
4.c3380360.chunk.js:sourcemap:1149 API_TRIES_EXHAUSTED
2.55c473cc.chunk.js:sourcemap:2 API tries exhausted TBL2-4e8513f0-5b20-4666-86d2-d96429b53e97 Object
2.55c473cc.chunk.js:sourcemap:2 getSystemUpdateInfo did not return. Usually means no connection
2.55c473cc.chunk.js:sourcemap:2 OtaStopInstall
2.55c473cc.chunk.js:sourcemap:2 TBL3 >>> {"Query":"GetInstalledApks"}
2.55c473cc.chunk.js:sourcemap:2 TBL1 >>> {"Query":"Version"}
4.c3380360.chunk.js:sourcemap:1149 API_TRIES_EXHAUSTED
2.55c473cc.chunk.js:sourcemap:2 API tries exhausted TBL3-106ee752-8077-4631-8cb3-60a347d2c258 Object

Lenovo Tablet Logs:
I think this is the cause.
06-29 16:07:32.682  1000   570   654 W SurfaceFlinger: Attempting to set client state on removed layer: Splash Screen com.penumbrainc.mvihealth.tablet.offlinetest#0
06-29 16:07:32.682  1000   570   654 W SurfaceFlinger: Attempting to destroy on removed layer: Splash Screen com.penumbrainc.mvihealth.tablet.offlinetest#0
06-29 16:07:32.847  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:33.865  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:34.145 10041  1372  1372 D chengwb1: hideNavigationBar() mNavigationBarView = com.android.systemui.statusbar.phone.NavigationBarFrame{2a7ce8e V.E...... ........ 0,0-1920,72 #7f0a0247 app:id/navigation_bar_frame}
06-29 16:07:34.145 10041  1372  1372 D chengwb1: hideNavigationBar() mNavigationBar = NavigationBarFragment{1afb329 #0 id=0x7f0a0247 NavigationBar}
06-29 16:07:34.155  1000   570  1213 W SurfaceFlinger: Attempting to destroy on removed layer: 508d58a NavigationBar#0
06-29 16:07:34.314  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:34.315  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:36.778  root   555   587 E ANDR-PERF-MPCTL: Invalid profile no. 0, total profiles 0 only
06-29 16:07:37.629  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:37.630  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:37.863  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:38.864  1000   570   570 I chatty  : uid=1000(system) /system/bin/surfaceflinger identical 5 lines
06-29 16:07:38.864  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:41.785  root   555   587 E ANDR-PERF-MPCTL: Invalid profile no. 0, total profiles 0 only
06-29 16:07:41.968 10057 13296 13346 D NetworkSecurityConfig: No Network Security Config specified, using platform default
06-29 16:07:42.033 10057 13296 13378 I LogMessage (level Message): [2] org.java_websocket.WebSocketImpl@333896c local port:8887, remote address:/::1:45062 entered the room!
06-29 16:07:42.038 10057 13296 13379 I LogMessage (level Message): [2] org.java_websocket.WebSocketImpl@6589b35 local port:8886, remote address:/::1:39118 entered the room!
06-29 16:07:42.050 10057 13296 13378 I System.out: org.java_websocket.WebSocketImpl@333896c: {"Ping":"2022-06-29T23:07:41.649Z"}
06-29 16:07:42.131  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:42.132  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:42.361 10057 13296 13405 I LogMessage (level Message): raw socket string message: 
06-29 16:07:42.361 10057 13296 13405 I LogMessage (level Message): {"Pong":"2022-06-29T23:07:43.131Z"}
06-29 16:07:42.414 10057 13296 13378 I System.out: org.java_websocket.WebSocketImpl@333896c: {"Query":"Version","MsgId":"TBL1-4afd97e3-e695-48dc-a19d-9195c05efa9d"}
06-29 16:07:42.573 10042  2587  2683 I WorkerManager: dispose()
06-29 16:07:42.574 10042  2587  2683 W ThreadPoolDumper: Queue length for executor EventBus is now 11. Perhaps some tasks are too long, or the pool is too small.
06-29 16:07:42.800  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:42.801  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:43.421 10057 13296 13378 I System.out: org.java_websocket.WebSocketImpl@333896c: {"Ping":"2022-06-29T23:07:43.410Z"}
06-29 16:07:43.512 10057 13296 13405 I LogMessage (level Message): raw socket string message: 
06-29 16:07:43.512 10057 13296 13405 I LogMessage (level Message): {"Pong":"2022-06-29T23:07:44.280Z"}
06-29 16:07:44.196  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:44.197  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:44.686 10057 13296 13378 I System.out: org.java_websocket.WebSocketImpl@333896c: {"Query":"SystemUpdateInfo","MsgId":"TBL2-4e8513f0-5b20-4666-86d2-d96429b53e97"}
06-29 16:07:44.880  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:44.881  1000   570   570 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 16:07:45.006 10057 13296 13378 I System.out: org.java_websocket.WebSocketImpl@333896c: {"Ping":"2022-06-29T23:07:45.000Z"}
06-29 16:07:46.789  root   555   587 E ANDR-PERF-MPCTL: Invalid profile no. 0, total profiles 0 only
06-29 16:07:51.038 10057 13296 13378 I System.out: org.java_websocket.WebSocketImpl@333896c: {"Ping":"2022-06-29T23:07:51.033Z"}
06-29 16:07:51.799  root   555   587 E ANDR-PERF-MPCTL: Invalid profile no. 0, total profiles 0 only
06-29 16:07:52.673 10015  2089  2089 I chatty  : uid=10015 com.google.android.gms.persistent expire 4 lines
06-29 16:07:55.501  root   774   916 E storaged: getDiskStats failed with result NOT_SUPPORTED and size 0
06-29 16:07:56.808  root   555   587 E ANDR-PERF-MPCTL: Invalid profile no. 0, total profiles 0 only
06-29 16:07:57.048 10057 13296 13378 I System.out: org.java_websocket.WebSocketImpl@333896c: {"Ping":"2022-06-29T23:07:57.040Z"}
06-29 16:07:57.537 10057 13296 13378 I System.out: org.java_websocket.WebSocketImpl@333896c: {"Query":"Version","MsgId":"TBL1-4afd97e3-e695-48dc-a19d-9195c05efa9d"}
06-29 16:07:59.720 10057 13296 13378 I System.out: org.java_websocket.WebSocketImpl@333896c: {"Query":"GetInstalledApks","MsgId":"TBL3-106ee752-8077-4631-8cb3-60a347d2c258"}

Actual SocketException
06-29 16:08:23.292 10057 13296 13405 W System.err: java.net.SocketException: Connection reset
06-29 16:08:23.293 10057 13296 13405 W System.err: 	at java.net.SocketInputStream.read(SocketInputStream.java:215)
06-29 16:08:23.293 10057 13296 13405 W System.err: 	at java.net.SocketInputStream.read(SocketInputStream.java:144)
06-29 16:08:23.293 10057 13296 13405 W System.err: 	at java.io.DataInputStream.readFully(DataInputStream.java:198)
06-29 16:08:23.293 10057 13296 13405 W System.err: 	at java.io.DataInputStream.readShort(DataInputStream.java:317)
06-29 16:08:23.293 10057 13296 13405 W System.err: 	at com.mvihealth.sockethost.SocketRelayReplyThread.run(SocketRelayReplyThread.java:35)
06-29 16:08:23.293 10057 13296 13405 E LogMessage (level Error): ###API Socket Exception###
06-29 16:08:23.293 10057 13296 13405 E LogMessage (level Error): java.net.SocketException: Connection reset
06-29 16:08:23.293 10057 13296 13405 E LogMessage (level Error): Connection reset
06-29 16:08:23.295 10057 13296 13405 E LogMessage (level System): Closing data connectionSocket[address=/10.220.8.103,port=44426,localPort=8082]
06-29 16:08:23.959 10057 13296 13398 E LogMessage (level System): #2 api connection from /10.220.8.103:36792
06-29 16:08:23.960 10057 13296 13397 E LogMessage (level System): #1 screen casting connection from /10.220.8.103:49572
06-29 16:08:23.961 10057 13296 13398 E LogMessage (level System): Sending kill message to Socket Relay Thread socketRelayThread_1


HTC HMD Logs:
06-29 23:07:55.785  1002   878   878 I android.hardware.bluetooth@1.0-service: Registering SAR service
06-29 23:07:55.786  1000   887   887 E light   : light_open lights bluetooth failed: -22
06-29 23:07:55.786  1000   887   887 E light   : Light passthrough failed to load legacy HAL.
06-29 23:07:55.786  1000   887   887 E light   : light_open lights wifi failed: -22
06-29 23:07:55.786  1000   887   887 E light   : Light passthrough failed to load legacy HAL.
06-29 23:07:55.787  1000   887   887 I ServiceManagement: Registered android.hardware.light@2.0::ILight/default (start delay of 107ms)
06-29 23:07:55.787  1000   887   887 I ServiceManagement: Removing namespace from process name android.hardware.light@2.0-service to light@2.0-service.
06-29 23:07:55.787  1000   887   887 I         : Registration complete for android.hardware.light@2.0::ILight/default.
06-29 23:07:55.789  1000   899   899 I ServiceManagement: Registered vendor.qti.hardware.display.allocator@3.0::IQtiAllocator/default (start delay of 98ms)
06-29 23:07:55.789  1000   899   899 I ServiceManagement: Removing namespace from process name vendor.qti.hardware.display.allocator-service to allocator-service.
06-29 23:07:55.789  1000   899   899 I qdgralloc: Initialized qti-allocator
06-29 23:07:55.790  root   933   933 E vendor.rmt_storage: Mmap Failed for rmts...pausing execution!
06-29 23:07:55.793  1047   879   879 I android.hardware.camera.provider@2.4-service: CameraProvider@2.4 legacy service is starting.
06-29 23:07:55.794  1000   920   947 I pd-mapper-svc: Starting servloc server
06-29 23:07:55.795  1000   890   890 I android.hardware.power@1.2-service: Power HAL Service 1.2 is starting.
06-29 23:07:55.795  1000   890   890 I QTI PowerHAL: Initing
06-29 23:07:55.798  1002   878   878 E vendor.qti.hardware.bluetooth_sar@1.0-BluetoothSar: HIDL_FETCH_IBluetoothSar
06-29 23:07:55.798  1000   890   890 I ServiceManagement: Registered android.hardware.power@1.2::IPower/default (start delay of 108ms)
06-29 23:07:55.798  1000   890   890 I ServiceManagement: Removing namespace from process name android.hardware.power@1.2-service to power@1.2-service.
06-29 23:07:55.798  1000   890   890 I android.hardware.power@1.2-service: Power Service is ready
06-29 23:07:55.799  1000   921   950 I PerMgrSrv: QMI service start
06-29 23:07:55.799 media   884   884 I ServiceManagement: Registered android.hardware.drm@1.2::IDrmFactory/widevine (start delay of 119ms)
06-29 23:07:55.799 media   884   884 I ServiceManagement: Removing namespace from process name android.hardware.drm@1.2-service.widevine to drm@1.2-service.widevine.
06-29 23:07:55.799  root   901   901 E         : IOP-HAL: loading library is done
06-29 23:07:55.799  1000   903   903 I ServiceManagement: Registered vendor.qti.hardware.qteeconnector@1.0::IAppConnector/default (start delay of 109ms)
06-29 23:07:55.799  1000   903   903 I ServiceManagement: Removing namespace from process name vendor.qti.hardware.qteeconnector@1.0-service to qteeconnector@1.0-service.
06-29 23:07:55.800  1000   896   896 I ServiceManagement: Registered vendor.qti.esepowermanager@1.0::IEsePowerManager/default (start delay of 110ms)
06-29 23:07:55.800  1000   896   896 I ServiceManagement: Removing namespace from process name vendor.qti.esepowermanager@1.0-service to esepowermanager@1.0-service.
06-29 23:07:55.800  1000   896   896 I vendor.qti.esepowermanager@1.0-service: Registration complete for vendor.qti.esepowermanager@1.0::IEsePowerManager/default.
06-29 23:07:55.800  1000   909   909 D         : tui_comm: svc service starting :)
06-29 23:07:55.800  1000   907   907 D QSEECOMAPI: QSEECom_get_handle sb_length = 0x2800
06-29 23:07:55.801  1000   907   907 D QSEECOMAPI: App is not loaded in QSEE
06-29 23:07:55.801  1000   907   907 E QSEECOMAPI: Error::Cannot open the file /vendor/firmware_mnt/image/soter64.mdt errno = 2
06-29 23:07:55.801  1000   907   907 E QSEECOMAPI: Error::Loading image failed with ret = -1
06-29 23:07:55.801  1000   907   907 D QSEECOMAPI: QSEECom_get_handle sb_length = 0x2800
06-29 23:07:55.801  1000   907   907 D QSEECOMAPI: App is not loaded in QSEE
06-29 23:07:55.801  1000   907   907 E QSEECOMAPI: Error::Cannot open the file /vendor/firmware_mnt/image/soter.mdt errno = 2
06-29 23:07:55.801  1000   907   907 E QSEECOMAPI: Error::Loading image failed with ret = -1
06-29 23:07:55.801  1000   907   907 E SoterUtils: QSEECom_start_app failed


=========================================================================================== 

PLAT-5615 | Crash Suspected to be:

TV Target String:
2.b0c04c1e.chunk.js:2 API timeout TBL19-52e9e1c3-4d8a-48b9-b453-bc0964cf6646 Object
2.b0c04c1e.chunk.js:2 TBL19 >>> {"Command":"LaunchApk","Args":{"ApkName":"com.RealSystem.WallRideGames.PublicQworks"},"hasPeer":true,"peer":null}
2.b0c04c1e.chunk.js:2 onDeviceKey volumeDown 1
2.b0c04c1e.chunk.js:2 onDeviceKey volumeDown 0
2.b0c04c1e.chunk.js:2 onDeviceKey volumeDown 0
2.b0c04c1e.chunk.js:2 Did not receive ApkLaunched. com.RealSystem.WallRideGames.PublicQworks Try number 1
2.b0c04c1e.chunk.js:2 TBL20 >>> {"Query":"CurrentApkInfo"}
2.b0c04c1e.chunk.js:2 TBL19 >>> {"Command":"LaunchApk","Args":{"ApkName":"com.RealSystem.WallRideGames.PublicQworks"},"hasPeer":true,"peer":null}
2.b0c04c1e.chunk.js:2 API timeout TBL20-74eca905-a173-4de7-9d8f-9352bafb0b8f Object
2.b0c04c1e.chunk.js:2 TBL20 >>> {"Query":"CurrentApkInfo"}
2.b0c04c1e.chunk.js:2 API tries exhausted TBL19-52e9e1c3-4d8a-48b9-b453-bc0964cf6646 Object
2.b0c04c1e.chunk.js:2 [GAME} Wed Jun 29 2022 17:43:41 GMT-0700 (Pacific Daylight Time) Timeout sending request to HMD after 15000ms Object
r.<computed> @ 2.b0c04c1e.chunk.js:2
2.b0c04c1e.chunk.js:2 HMD disconnected
2.b0c04c1e.chunk.js:2 [SENSORS]cancel sensorWorkflowSaga 
2.b0c04c1e.chunk.js:2 [SENSORS]finally sensorWorkflowSaga
2.b0c04c1e.chunk.js:2  [Error] ###API Socket Exception###java.net.SocketException: Connection timed outConnection timed out
r.<computed> @ 2.b0c04c1e.chunk.js:2
2.b0c04c1e.chunk.js:2  [System] Closing data connectionSocket[address=/10.220.8.102,port=49098,localPort=8082]
r.<computed> @ 2.b0c04c1e.chunk.js:2
2.b0c04c1e.chunk.js:2  [Error] ###Error Sending Message to Tablet###java.net.SocketException: Socket closedSocket closed


Lenovo Tablet Logs:
06-29 17:42:56.450 10079  4835  4916 I System.out: org.java_websocket.WebSocketImpl@158e36b: {"Command":"LaunchApk","Args":{"ApkName":"com.RealSystem.WallRideGames.PublicQworks"},"MsgId":"TBL19-52e9e1c3-4d8a-48b9-b453-bc0964cf6646"}
06-29 17:42:56.552  1000  1142  1303 W BestClock: java.time.DateTimeException: Missing NTP fix
06-29 17:42:56.575  1000  1142  1303 W BestClock: java.time.DateTimeException: Missing NTP fix
06-29 17:42:56.577  1000  1142  1304 W BestClock: java.time.DateTimeException: Missing NTP fix
06-29 17:42:59.681 10079  4835  4916 I System.out: org.java_websocket.WebSocketImpl@158e36b: {"Ping":"2022-06-30T00:42:59.677Z"}
06-29 17:43:00.004 10041  1370  1370 D KeyguardUpdateMonitor: received broadcast android.intent.action.TIME_TICK
06-29 17:43:00.005 10041  1370  1370 D KeyguardUpdateMonitor: handleTimeUpdate
06-29 17:43:01.618 10079  4835  4953 E LogMessage (level Error): ###Image Socket Timeout Exception###
06-29 17:43:01.618 10079  4835  4953 E LogMessage (level Error): Read timed out
06-29 17:43:01.619 10079  4835  4953 E LogMessage (level System): Closing image connectionSocket[address=/10.220.8.102,port=42662,localPort=8080]
06-29 17:43:05.729 10079  4835  4916 I System.out: org.java_websocket.WebSocketImpl@158e36b: {"Ping":"2022-06-30T00:43:05.722Z"}
06-29 17:43:06.246 10015  2085  4992 E memtrack: Couldn't load memtrack module
06-29 17:43:06.247 10015  2085  4992 W android.os.Debug: failed to get memory consumption info: -1
06-29 17:43:06.787 10015  2374  4993 E memtrack: Couldn't load memtrack module
06-29 17:43:06.787 10015  2374  4993 W android.os.Debug: failed to get memory consumption info: -1
06-29 17:43:11.610 10079  4835  4916 I System.out: org.java_websocket.WebSocketImpl@158e36b: {"Command":"LaunchApk","Args":{"ApkName":"com.RealSystem.WallRideGames.PublicQworks"},"hasPeer":true,"peer":null,"MsgId":"TBL19-52e9e1c3-4d8a-48b9-b453-bc0964cf6646"}
06-29 17:43:11.734 10079  4835  4916 I System.out: org.java_websocket.WebSocketImpl@158e36b: {"Ping":"2022-06-30T00:43:11.729Z"}
06-29 17:43:14.859  1000   567   567 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 17:43:14.861  1000   567   567 I ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
06-29 17:43:15.984  1000  1142  1293 D WindowManager: KeyEvent:25
06-29 17:43:16.118  1000  1142  1293 W InputDispatcher: Excessive delay in interceptKeyBeforeQueueing; took 131 ms
06-29 17:43:16.119  1000  1142  1293 D WindowManager: KeyEvent:26
06-29 17:43:16.506  1000  1142  1293 D WindowManager: KeyEvent:25
06-29 17:43:16.514  1000  1142  1293 D WindowManager: KeyEvent:26
06-29 17:43:17.488  1000  1142  1293 D WindowManager: KeyEvent:25
06-29 17:43:17.656  1000  1142  1293 D WindowManager: KeyEvent:26
06-29 17:43:17.717  1000  1142  1650 D MediaSessionService: dispatchVolumeKeyEvent, pkg=com.penumbrainc.mvihealth.tablet.offlinestage, pid=4835, uid=10079, asSystem=true, event=KeyEvent { action=ACTION_DOWN, keyCode=KEYCODE_VOLUME_DOWN, scanCode=114, metaState=0, flags=0x8, repeatCount=0, eventTime=334426, downTime=334426, deviceId=6, source=0x101 }
06-29 17:43:17.730  1000  1142  1650 D MediaSessionService: Adjusting null by -1. flags=4113, suggestedStream=-2147483648, preferSuggestedStream=false
06-29 17:43:17.739 10041  1370  1526 I vol.Events: writeEvent active_stream_changed STREAM_MUSIC
06-29 17:43:17.739  1000  1142  1650 D MediaSessionService: dispatchVolumeKeyEvent, pkg=com.penumbrainc.mvihealth.tablet.offlinestage, pid=4835, uid=10079, asSystem=true, event=KeyEvent { action=ACTION_UP, keyCode=KEYCODE_VOLUME_DOWN, scanCode=114, metaState=0, flags=0x28, repeatCount=0, eventTime=334599, downTime=334426, deviceId=6, source=0x101 }
06-29 17:43:17.739  1000  1142  1650 D MediaSessionService: Adjusting null by 0. flags=4116, suggestedStream=-2147483648, preferSuggestedStream=false


HTC HMD Logs:
06-30 00:41:16.497  1000  1604  1724 E DefaultPermGrantPolicy: PackageNot found: com.RealSystem.WallrideGames.PublicQworks
06-30 00:41:16.497  1000  1604  1724 E DefaultPermGrantPolicy: android.content.pm.PackageManager$NameNotFoundException: com.RealSystem.WallrideGames.PublicQworks

=========================================================================================== 

PLAT-5599 | Crash Suspected to be:


TV Target String:


Lenovo Tablet Logs:


HTC HMD Logs:
