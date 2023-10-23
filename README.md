
# Assignment 1 - Lip Sync Model

This repository contains the notebook which if run in collab in GPU along with the video and audio files in the same local depository as notebook (upload audio and video files in collab env if doing in collab) will give the resulted video in result folder of Wav2Lip directory downloaded with notebook when you run the first cell.

Some problems with the videos I faced due to which other models I can't use are -
1. So the video didn't contain a face all the time due to which models like Wav2Lip will not seamlessly edit the whole video and you will find a mouth appearance in that frame where the face is not there. One remedy is trimming that part after the model gives the resultant video and replacing that part with the original clip so the moth appearance does not appear.
2.  I tried more advanced models like Wav2lip- HQ and Wav2lip - Super but in the  first it required the face in every frame of the video to work and in other it did not require the audio file to lip sync on the video but the video of the person saying the dub language so since I have only audio I cannot use that model too. 

## Suggestion-

1. The problem of face to be there in Wav2lip can be resolve by making some pipeline which take the frame from video where face is there and lip sync that parts individually and then stiching them together.Since due to time constraint I cannot implement this idea.

2. Also due to time constraint cannot add pipelene in AI model which I share so that it can edit the non face part from video by replacing it with original clip in this way it will not show mouth appearence which is coming in the video. This can be the soln for this video.

## About videos

So I have attached 2 video one with Wav2lip and other with Wav2lip-GAN . First one is good for syncing lips but quality of video reduces whereas second one increases the quality but little non-noticible voice quality reduces. Since this models are very old and not updated and the new models where facing problem as stated above , they are struggling to keep the lip sync in one place as the object of the video is moving a lot and in the Wav2lip repositroy it is suggested that models works well  with statuonary objects. The videos are in  the drive folder.Also vieos and audio are trimmed to 1 minute since that much model can do seamlessly.



