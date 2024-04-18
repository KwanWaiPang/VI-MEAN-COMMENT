 [comment]: <> (# Monocular Dense Mapping)

 <h1 align="center"> Monocular Dense Mapping 测试版本 (仅供个人学习记录用)
  </h1>


[comment]: <> (  <h2 align="center">PAPER</h2>)
  <h3 align="center">
  <a href="https://raw.githubusercontent.com/dvorak0/VI-MEAN/master/ICRA17_1095_MS.pdf">Paper </a> 
  | <a href="https://github.com/dvorak0/VI-MEAN">Original Github Page</a>
  | <a href="https://github.com/arclab-hku/Event_based_VO-VIO-SLAM?tab=readme-ov-file#5-evi-sam">Testing Dataset</a>
  </h3>
  <div align="center"></div>

  * 为了方便本人使用，对代码做了修改(配置到20.04以及opencv4.0中)，源码请参见原github仓库~
  * 编译成功，但运行报错一堆，待解决。。。

~~~
  roslaunch stereo_mapper sample_all.launch
~~~

~~~
@inproceedings{yang2017real,
  title={Real-time monocular dense mapping on aerial robots using visual-inertial fusion},
  author={Yang, Zhenfei and Gao, Fei and Shen, Shaojie},
  booktitle={2017 IEEE International Conference on Robotics and Automation (ICRA)},
  pages={4552--4559},
  year={2017},
  organization={IEEE}
}
~~~