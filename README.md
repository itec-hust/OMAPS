# OMAPS

At present, the datasets used in piano transcription research include [MAPS dataset](https://amubox.univ-amu.fr/index.php/s/iNG0xc5Td1Nv4rR), [MAESTRO dataset](https://magenta.tensorflow.org/datasets/maestro) for audio transcription, and [MTA dataset](http://www.sfu.ca/akbari/MTA/Dataset) for video transcription. However, the dataset used for audio-visual fusion transcription has not been proposed yet. To evaluate the performance of different audio-video fusion models, we have established the OMAPS dataset. 

The **OMAPS (Ordinary MIDI Aligned Piano Sounds) dataset** was recorded from Yamaha electric piano P115 by a piano player. The Logitech C922 Pro HD stream webcam was used to record video and audio simultaneously. The Logitech camera is available in both 1080p/30fps and 720p/60fps video configurations. To ensure the resolution of the video, we used the 1080p/30fps configuration. The Logitech camera audio module’s sampling rate is 44100Hz. Since the recorded videos and piano MIDI files were out of sync, we manually aligned the exported MIDI files as annotations. The OMAPS dataset contains 106 different pieces for a total of 216 minutes, with an average of two minutes per piece. The amount of notes played per second is used to measure the playing speed. According to the playing speed, the OMAPS dataset is divided into a training set and a test set. The training set and the test set have the same playing speed distribution. The training set contains 80 videos, and the test set contains 26 videos, as shown in the table bellow.

| Split | Performance | Duration, minutes | Size, GB | Notes |
| ----- | ----- | ----- | ----- | ----- |
| Train | 80 | 123 | 3.18 | 60, 589 |
| Test | 26 | 53 | 1.03 | 19, 135 |
| Total | 106 | 176 | 4.22 | 79, 724|



Here is a picture of our recording environment. Yamaha P-115 piano and  logitech C922 PRO HD stream webcam are used for recording in an quiet room. You can have a look at OMAPS dataset under the OMAPS folder of this repository. The complete OMAPS dataset will be available when the paper is published. The test set is provided now!

<img src="pics/record.png" alt="record" style="zoom:24%;" />