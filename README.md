# Smart Queueing System

This System is used to count the number of people in a particular.

![](img/demo.png)

## Purpose

Intel's DevCloud provides a way to test edge computing applications on different types of hardwares like `FPGA`, `VPU`, `CPU` and `GPU` using the OpenVINO toolkit. This system leverages those Intel DevCloud's capabilities to test a Smart Queueing System edge application on the Intel's DevCloud.

## Directory Structure

```bash
.
├── Manufacturing_Scenario.ipynb
├── Transportation_Scenario.ipynb
├── Retail_Scenario.ipynb
├── img
│   └── demo.png
├── original_videos
│   ├── Manufacturing.mp4
│   ├── Retail.mp4
│   └── Transportation.mp4
├── output.tgz
├── person_detect.py
├── queue_job.sh
├── README.md
├── results
│   ├── manufacturing
│   │   ├── cpu
│   │   │   ├── output_video.mp4
│   │   │   └── stats.txt
│   │   ├── fpga
│   │   │   ├── output_video.mp4
│   │   │   └── stats.txt
│   │   ├── gpu
│   │   │   ├── output_video.mp4
│   │   │   └── stats.txt
│   │   └── vpu
│   │       ├── output_video.mp4
│   │       └── stats.txt
│   ├── retail
│   │   ├── cpu
│   │   │   ├── output_video.mp4
│   │   │   └── stats.txt
│   │   ├── fpga
│   │   │   ├── output_video.mp4
│   │   │   └── stats.txt
│   │   ├── gpu
│   │   │   ├── output_video.mp4
│   │   │   └── stats.txt
│   │   └── vpu
│   │       ├── output_video.mp4
│   │       └── stats.txt
│   └── transportation
│       ├── cpu
│       │   ├── output_video.mp4
│       │   └── stats.txt
│       ├── fpga
│       │   ├── output_video.mp4
│       │   └── stats.txt
│       ├── gpu
│       │   ├── output_video.mp4
│       │   └── stats.txt
│       └── vpu
│           ├── output_video.mp4
│           └── stats.txt
├── Choose the Right Hardware – Proposal.pdf
├── Create_Job_Submission_Script.ipynb
├── Create_Python_Script.ipynb
├── stderr.log
└── stdout.log
```

## Files Explanation:

* `person_detect.py`: The main file which runs inference on the frames by accepting the arguments passed by the job submitting script.
* `queue_job.sh`: The script which allows to submit it to intel's devcloud platform
* `Retail_Scenario.ipynb`: The testing of application on the retail scenario.
* `Transportation_Scenario.ipynb`: The testing of application on the Transportation scenario.
* `Manufacturing_Scenario.ipynb`: The testing of application on the Manufacturing scenario.
* `original_videos`: Testing videos
* `results`: The stats and resultant videos on different hardware have been saved here.