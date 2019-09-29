# 20-data

This repository contains training data and model from the events of [Connected-Autonomous-Driving Meetups](https://www.meetup.com/Connected-Autonomous-Driving/).
The training data are produced for (Donkey Car)[https://github.com/autorope/donkeycar]

## collection of training data

| tub             | records | track                   | description          | driving   | date     | model      | data quality    |
|----------------:|:-------:|:-----------------------:|:---------------------|:---------:|:--------:|:----------:|:--------------:|
| 36              |    9136 | 2 big track             | Bosch Solaris Course | Left      | 20190413 | Solaris2.h5 | [tubhist](https://github.com/connected-autonomous-mobilty/20-data/blob/master/images/tubhist_tub_36_19-04-13.png)|
| 19              |  ~11000 | 2 big track (clock wise)| Bosch Solaris Course | All       | 20190929 | none        | none |


## own data
```
(env) rainer@rbnano1:~/mycar/data$ for i in $(find . -maxdepth 1 -type d) ; do echo -n $i": " ; (find $i -type f | wc -l) ; done | sort
.: 142000
./tub_16_19-03-10: 21085
./tub_18_19-03-10: 20435
./tub_36_19-04-13: 18273
./tub_6_19-03-09: 25885
./tub_64_19-06-15: 6841
./tub_66_19-06-15: 6841
./tub_67_19-06-15: 6841
./tub_68_19-06-15: 6841
./tub_69_19-06-15: 6841
./tub_9_19-03-09: 22117
```


### old dataset 
[Tawn Kramer's big training dataset](https://s3.amazonaws.com/tawn-train/log_donkey/combined_donkey_tub_data.zip)

### August 7th, 2019
[Tawn Kramer pretrained](https://donkeycar.slack.com/archives/C4B69691N/p1561165380013700)
[model with 200+k images](https://drive.google.com/open?id=18Qfc_T5fpUmuTqXFZbJZrQhlf2l3S0VK)

[Tawn Kramers's new dataset](https://tawn-train.s3.amazonaws.com/log_donkey/lg_data.tar.gz)
content:
```~/mycar/data/lg_data$ 
for i in $(find . -maxdepth 1 -type d) ; do echo -n $i": " ; (find $i -type f | wc -l) ; done | sort
.: 1902040
./alley_vanmil_1: 7270
./alley_vanmil_2: 10326
./american_steel_adam_2: 3408
./american_steel_oak_data3_adam: 68423
./asphalt_75fov_centerline: 26076
./athena_rainer_bosch: 36482
./aws_reinvient_adam: 35620
./circuit_launch_adam_1: 19060
./circuit_launch_ed_1: 57414
./circuit_launch_ed_2: 61882
./driveai_data3_adam: 73476
./driveway_120fov_leftlane: 24002
./google_io_adam_1: 36640
./hive_cone_avoid_2: 111854
./hive_cone_avoid_3: 43186
./hive_cone_avoid: 9706
./hive_fast_driving_2: 58346
./hive_fast_driving: 40462
./hive_imu_fast_racing_2: 40506
./hive_imu_fast_racing: 37302
./hive_imu_left_lane_in_traffic: 87130
./hive_left_lane_driving: 71866
./hive_ps3_cam: 24070
./hive_right_lane_driving: 72078
./hive_wandering_in_traffic: 7814
./mapbox_locate_adam_1: 24072
./san_mateo_maker_faire_adam: 36004
./sd_history_center_llane_1: 67514
./sd_history_center_llane_2: 19702
./sd_history_center_llane_avoid: 59662
./seattle_hackathon_adam: 35796
./sim_gen_roads_pid_1_rl: 135878
./sim_gen_roads_pid_2_rl: 176292
./sim_warehouse_manual: 48132
./ucsd_afternoon: 19694
./ucsd_avg_drv: 28570
./ucsd_fast_track: 39014
./ucsd_mid_morn: 15206
./ucsd_morn: 34476
./ucsd_oscillate: 32490
./ucsd_outdoor_track_1: 45310
./ucsd_slow_driving: 19786
```
