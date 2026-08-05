# Pond Duck Strategy Code

```javascript
var scan_angle = 0;
var scan_increment = 10;
var movement_angle = 0;

while (true) {
  movement_angle += 2;
  swim(movement_angle, 100);
  var dist = scan(scan_angle, scan_increment);
  if (dist <= 70) {
    cannon(scan_angle, dist);
  } else {
    scan_angle += scan_increment;
  }
}
```
