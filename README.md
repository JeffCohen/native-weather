This app sucks.

Click the "Get Satellite Photo" button and it will get
your current location, but setting the state with the new
coordinates does not trigger a re-render.

Here's a snippet from the log file.  Notice that after the
initial render, subsequent button clicks do not trigger
re-rendering for some reason.

```
11:29:53 AM: Rendering...
11:29:53 AM: Image URL:
11:29:53 AM: https://maps.googleapis.com/maps/api/staticmap?center=48.864716,2.349014&zoom=15&size=300x200&maptype=hybrid&key=AIzaSyBrLfaqBHZNoiI8463XDdy57fJHiwA8vy4
11:29:55 AM: Button clicked!
11:29:55 AM: Object {
11:29:55 AM:   "accuracy": 5,
11:29:55 AM:   "altitude": 0,
11:29:55 AM:   "altitudeAccuracy": -1,
11:29:55 AM:   "heading": -1,
11:29:55 AM:   "latitude": 37.785834,
11:29:55 AM:   "longitude": -122.406417,
11:29:55 AM:   "speed": -1,
11:29:55 AM: }
11:30:09 AM: Button clicked!
11:30:09 AM: Object {
11:30:09 AM:   "accuracy": 5,
11:30:09 AM:   "altitude": 0,
11:30:09 AM:   "altitudeAccuracy": -1,
11:30:09 AM:   "heading": -1,
11:30:09 AM:   "latitude": 37.785834,
11:30:09 AM:   "longitude": -122.406417,
11:30:09 AM:   "speed": -1,
11:30:09 AM: }
```
