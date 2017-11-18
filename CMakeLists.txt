cmake_minimum_required(VERSION 2.8.3)
project(gbx_ros_bridge_msgs)

find_package(catkin REQUIRED COMPONENTS
  std_msgs
  geometry_msgs
  message_generation
)

## Generate messages in the 'msg' folder
add_message_files(
  FILES
  TxId.msg
  BaseTime.msg
  TriggerTime.msg
  ObservablesMeasurementTime.msg
  GnssObservables.msg
  GnssObservablesSegment.msg
  NavigationSolution.msg
  TransmitterInfo.msg
  TransmitterInfoSegment.msg
  StatusMessage.msg
  Ephemeris.msg
  Almanac.msg
  Bitcontainer.msg
  Info.msg
  Status.msg
  GPStoUTC.msg
  Coda.msg
  Radar.msg
  RadarTarget.msg
  RadarConfig.msg
  Attitude2D.msg
  Attitude3D.msg
  SingleBaselineRTK.msg
  MultiBaselineRTKAttitude2D.msg
  MultiBaselineRTKAttitude3D.msg
  Imu.msg
  ImuConfig.msg
)

generate_messages(
  DEPENDENCIES
  std_msgs
  geometry_msgs
)

catkin_package( CATKIN_DEPENDS 
    std_msgs 
    geometry_msgs
    message_runtime)

