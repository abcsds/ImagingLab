Paradigm:
1. Welcome screen
2. Instructions
3. Main loop:
  - Two conditions at random:
   - Press with right hand
   - Press with left hand
  Repeat 20 times each.
4. End screen

12 min
```
from pylsl import StreamInfo, StreamOutlet

info = StreamInfo('PsychopyStream', 'Markers', 1, 0, 'string', '42')
outlet = StreamOutlet(info)

outlet.push_sample("Welcome")
```
