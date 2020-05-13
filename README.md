# PhoneSensorMath
A repository of math-oriented projects that incorporate data from sensors
found in typical cell phones. The projects are all rendered in jupyter
notebooks that have markdown annotations. To use these, download the .zip
file of the repository, load the .ipynb file into jupyter, modify to suit
your needs. Please visit https://github.com/schuelaw/PhoneSensorMath for
the latest version.

There are a couple of ways of getting access to jupyter. The [Anaconda
distribution](https://www.anaconda.com/download/) comes with a jupyter
interface. Download and install the software, run the _Anaconda Navigator_
and click the ```Launch``` button under the jupyter notebook icon. This
will create a window in your browser that contains a fully functioning jupyter
environment.

Alternatively, you can avoid installing software on your computer by
creating a free account at [CoCalc](https://cocalc.com/). Just login,
create a project, upload the example files and run them in your browser.

Collaborations and ideas for projects are welcome. Message at
SensorMath@gmail.com

## GPS Fastest Mile Analysis
__(FILE: PSM GPS Fastest Mile Analysis)__ This notebook describes the
collection and analysis of GPS data recorded during an exercise
run/walk/bike. The analysis allows one to determine the fastest mile within
the longer exercise course. The notebook is documented so that other
lengths and units (i.e. kilometer) can be considered. Such an analysis might
accompany an introductory calculus curriculum about time vs. distance.

__(FILE: PSM GPS Plotly Mapping Example - Mapbox)__ This notebook accepts
recorded GPS data and plots it on a map.  The notebook uses the
__[Plotly](https://plot.ly)__ plotting library and the
__[Mapbox](https://www.mapbox.com/)__ mapping library. Both libraries are
free for non-commercial use (with some minor limitations) and are suitable
for use by students and instructors in academic data science
applications.

## Accelerometer Frequency Analysis
__(FILE: PSM Accelerometer Frequency Analysis)__ This notebook describes
the collection and analysis of phone accelerometer data recorded while the
phone rested on a clothes washer during its spin cycle. The rate of spin is
determined by using the discrete Fourier transform and identifying the
dominant frequency of vibration in the accelerometer data. This analysis
might accompany an engineering math course as it discusses the discrete
Fourier transform.

## Calculating Height with the Accelerometer
__(FILE: PSM Calculating Height)__ This notebook describes
the collection and analysis of accelerometer data recorded while a phone rose
from the floor to the height of a person. Then the height is calculated using
calculus and approximating the integral of the acceleration data to find velocity
and then again approximating the integral of the velocity data to find the
change in posiiton, or height of the person. This analysis could accompany
a Calculus class at many levels as well as a Physics class.

## Physics Toolbox Sensor Suite
The examples in this repository use data collected with a free app called
the [Physics Toolbox Sensor Suite](https://www.vieyrasoftware.net/). There
may be other apps out there that do the same thing, but this one is pretty
good. That said, there are a few quirks some of which are discussed below.
You are encouraged to do a lot of test recordings with different sensors
before committing a lot of time to a long recording. The GPS sensor
recording is particularly prone to failure unless you get things just
right.

Tips about recording with the physics toolbox sensor suite. I use the app
on a OnePlus 3T phone.  A lot of phones, like mine, want to conserve
battery power and aggressively try to put idle apps to sleep. This _may_
cause your recordings of various sensors either to fail to start, or to
shutdown prematurely. The behavior is highly dependent on the phone. Make
sure you understand your phone quirks _before_ you go out on a long
recording only to find that the recording stopped halfway through the
effort. Here are a few things that I've learned about my own phone. My
knowledge of iPhone behavior in this area is practically zero. (__Note:__
if you have tips you'd like to add to this list, please send them to me.)

1. Lots of Android phones have a battery optimization section in the
   settings. This provides an app-by-app listing of battery optimization.
   It's wise to disable all battery optimization on whatever app you're
   using to record sensors.

1. GPS recording, go to the GPS sensor page in the app, go into "advanced
   stats" wait until GPS lock, go back to the initial GPS screen, hit
   record, then recording is happening. On my phone, it is necessary to
   keep that screen selected and to keep the screen on during the _entire_
   recording. Fortunately, there is a setting to "Keep the screen on".
   Keeping the screen on and carefully putting the phone into a waistband
   or armband carrier has yielded the most reliable recordings.
   
   Sometimes, if the GPS signal is lost during the recording, the recording
   will stop without notice.

1. Accelerometer (an other sensor) recording seems to work pretty robustly
   by just hitting the record button, note that it generates a lot of
   readings since the sample rate is around 200Hz (at least on my phone).

1. Multirecording, works as expected for most sensor combinations. I have
   not been able to add GPS to a multirecording.

1. In general, most of the issues seem to center around getting the GPS to
   lock and _stay_ locked. Getting the GPS going, bringing up the GPS
   screen, and keeping the phone screen on during recording seems to be the
   most reliable recording method. Your results may vary.
