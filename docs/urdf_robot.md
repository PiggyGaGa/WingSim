## WingSim支持URDF机器人

## 流程

设置`robot`模式，演示视频中的Settings.json文件配置如下：

```
{
  "SeeDocsAt": "https://github.com/Microsoft/AirSim/blob/main/docs/settings.md",
  "SettingsVersion": 1.2,
  "Clockspeed": 0.5,
  "SimMode": "Robot",
  "PawnPaths": {
    "DefaultRobot": {
      "PawnBP": "Class'/AirSim/Robot/RobotPawn.RobotPawn_C'"
    }
  },
  "Vehicles": {
    "robot_1": {
      "VehicleType": "robot",
      "DisplayName": "pi",
      "AutoCreate": true,
      "Sensors": {
        "Imu": {
          "SensorType": 2,
          "Enabled": true
        }
      },
      "Cameras": {
        "front_center_custom": {
          "CaptureSettings": [
            {
              "PublishToRos": 1,
              "ImageType": 0,
              "Width": 640,
              "Height": 480,
              "FOV_Degrees": 120,
              "DepthOfFieldFstop": 2.8,
              "DepthOfFieldFocalDistance": 200.0,
              "DepthOfFieldFocalRegion": 200.0,
              "TargetGamma": 1.5
            }
          ],
          "X": 0.0,
          "Y": 0,
          "Z": -0.30,
          "Pitch": 0,
          "Roll": 0,
          "Yaw": 0
        }
      }
    },
    "robot_2": {
      "VehicleType": "robot",
      "DisplayName": "pi",
      "AutoCreate": true,
      "Sensors": {
        "Imu": {
          "SensorType": 2,
          "Enabled": true
        }
      },
      "X": 1.50,
      "Y": 0,
      "Z": 0.0,
      "Pitch": 0,
      "Roll": 0,
      "Yaw": 0
    },
    "robot_3": {
      "VehicleType": "robot",
      "DisplayName": "pi",
      "AutoCreate": true,
      "Sensors": {
        "Imu": {
          "SensorType": 2,
          "Enabled": true
        }
      },
      "X": 0.0,
      "Y": 1.0,
      "Z": 0.0,
      "Pitch": 0,
      "Roll": 0,
      "Yaw": 0
    },
    "robot_4": {
      "VehicleType": "robot",
      "DisplayName": "pi",
      "AutoCreate": true,
      "Sensors": {
        "Imu": {
          "SensorType": 2,
          "Enabled": true
        }
      },
      "X": 1.0,
      "Y": 1.0,
      "Z": 0.0,
      "Pitch": 0,
      "Roll": 0,
      "Yaw": 0
    }
  }
}

```