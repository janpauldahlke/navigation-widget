--

###gesture based Navgiation -- a proof of concept

---will work only on smartphones with motion sensors!  
(hopefully it will perform well with the given MDN-api to grab all types of this kind of smartphones) 
minimum requirement. it should run at least on Andro5+/iOS8.1+

--
there is a widget one can open/close activate on demand on every given webpage.
if the widget is active the normal behavior of navigation on the site will feel completely different

- it needs to run in browser and not as app! (goal to achive is to make it work in html pages)

![Image of foo]
(https://dev.opera.com/articles/w3c-device-orientation-api/device-gamma.png)


--example

WHEN:<br/>
&nbsp;&nbsp;there is a standard html page and the user wants to interact with one of it's elements<br/>
WHEN:<br/>
&nbsp;&nbsp;activates widget on page<br/>
&nbsp;&nbsp;AND the user performs a gesture<br/>
THEN:<br/>
&nbsp;&nbsp;the navigation reacts on the user based command<br/>
&nbsp;&nbsp;(depending on the implemention of tzhe ruleset)<br/>


###rulesets: (these are model-thoughts that can be combined in the controller)
1st throw ruleset (these are examples and not finished yet)
- tilt right -- browse right hand content --deeper nested 
- tilt left -- browse left handf content --higher nodes
- shake -- reset to normal state // close lightbox
- knock -- open last state of page(? 


###2DO
-coding:
  - write(or steal) a simple html environment
  - make navigation switchable / widget charakter!
  - bind some navigational actions to gestures
  - 1.) 360° turn in canvas - skybox like
  - 2.) go level deeper/higher
  - 3.) slide with gesture 
  - 4.) raise quantity of some anything
  - 5.) feel free to add more usecases

-concept:
  - create a simple ruleset that key/values (maps) gesture/action


-knowledge:
  - research on deviceOrientation events
  - research on term "nested sets"


###Links
- https://developer.mozilla.org/en-US/docs/Web/API/Detecting_device_orientation
- https://github.com/dorukeker/gyronorm.js
- https://developer.android.com/guide/topics/sensors/sensors_motion.html


list of possible events: 

(!! i looked those up at android events, its still questionable if these events also occur on window.Events)

- orientation (x-y-z) 
- gyroscope (x-y-z: rotation)
- rotation (..)
- gravity (force of g on x-y-z-axis)
- accelaration(orce of g on x-y-z-axis -- but also contains gravity)
