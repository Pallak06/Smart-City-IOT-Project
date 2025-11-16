🟦 Fire System

IF fireDetected → FireMonitor.ON

IF FireMonitor.ALARM → Sprinkler.ON

IF noFire → Sprinkler.OFF


🟨 Street Lighting

IF night(lowLight) → Lamp.ON

IF day(brightLight) → Lamp.OFF

IF motionDetected → Lamp.brightness = HIGH


🔴 Security System

IF motionDetected → Camera.record()

IF motionDetected → Siren.ON

IF noMotion → Siren.OFF & Camera.stop


🟩 Alerts

IF fireAlarm → SendAlert(Tablet)

IF motionDetected → SendAlert(Tablet)
