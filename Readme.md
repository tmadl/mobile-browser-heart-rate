In-browser heart rate estimation on smartphones
=============

![logo](press.png)

Research-grade JavaScript code for estimating a users current heart rate on a smartphone from within the browser, using accelerometer sensors.
Acceleration is obtained using `DeviceMotionEvent', the signal is smoothed using [Savitzky-Golay filtering](https://en.wikipedia.org/wiki/Savitzky%E2%80%93Golay_filter) on two timescales (slow y-movement - breathing and fast y-movement - heart beat), slow breathing movements are subtracted, and peaks are counted in the remaining signal to obtain an approximate beat frequency.

This is an unrefined proof of concept (parameters not tuned, accuracy not verified, speed not optimized, etc.). Tested on Chrome and Firefox mobile.