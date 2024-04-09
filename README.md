# Kiểm tra phạt nguội csgt.vn

Sử dụng selenium để kiểm tra phạt nguội trên [csgt.vn](https://www.csgt.vn/tra-cuu-phuong-tien-vi-pham.html)

## Example

```
from phatnguoi import VehicleChecker


number_plate = "98A15555"
vehicle_type = "CAR" # CAR, MOTOBIKE, ELECTRIC_BIKE
checker = VehicleChecker(number_plate, vehicle_type)
result = checker.check()
if result:
    base64_img = result.screenshot_as_base64
    dist = "screenshot.png"
    result.screenshot(dist)
else:
    print("Không tìm thấy kết quả !")
```
