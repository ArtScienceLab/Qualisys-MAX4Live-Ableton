# Max objects for MoCap -> Max (-> Ableton)

### 1. Qualisys-MAX4Live-Ableton.amxd
Max4Live plug-in to receive Qualisys OSC and control Ableton track parameters

This MAX4live patch is to be placed in the Ableton Live master track.
It receives OSC from Qualisys on port 45458 and controls ableton parameters:
- track start/stop
- track tempo (BPM)
- individual tracks volume (up to 5 tracks)
- master track volume
- panning 
- distortion of the track

Markers names and rigid bodies names need to be adjusted.

### 2. ReceiveSendMoCapOSC.maxpat
A stand-alone Max object to receive MoCap XYZ-data over OSC and send it back out (scaled, locally).
One can scale the a 'cube' in which to move a rigidbody and control a position over OSC.
Example: It can be used with the IOSONO system using a tweaked version of the IOSONO M4L patch in Ableton (To be found in: Iosono4Live/OSCin/IOSONO_2019_xyzOSC.amxd)

- IN: Mocap 10.10.141.14, ports: 22225/45454, rigidbody = Hand
- OUT XYZ data over OSC /soundobject0, /soundobject1, ... port = 1111
