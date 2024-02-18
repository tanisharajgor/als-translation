<div style="text-align: center;">
    <img src="https://github.com/tanisharajgor/als-translation/assets/54627422/6c21e9da-0ef5-4d7e-8197-85aa59d9e2dd" alt="g-labelled" style="display:inline; margin:0px; width:110px; height:110px;">
    <img src="https://github.com/tanisharajgor/als-translation/assets/54627422/c732fb25-9bc9-4a7e-aee1-4af4a381d80d" alt="e-labelled" style="display:inline; margin:0px; width:110px; height:110px;">
    <img src="https://github.com/tanisharajgor/als-translation/assets/54627422/31da3f7a-181a-4707-9dd3-a3e4f204888b" alt="s-labelled" style="display:inline; margin:0px; width:110px; height:110px;">
    <img src="https://github.com/tanisharajgor/als-translation/assets/54627422/c56cab93-8e76-46cd-8165-f840e811166d" alt="t-labelled" style="display:inline; margin:0px; width:110px; height:110px;">
    <img src="https://github.com/tanisharajgor/als-translation/assets/54627422/2def20f3-e6ff-4023-95b1-731f43cbd034" alt="u-labelled" style="display:inline; margin:0px; width:110px; height:110px;">
    <img src="https://github.com/tanisharajgor/als-translation/assets/54627422/6195edce-acde-432a-b9ec-c4774fe4aa20" alt="r-labelled" style="display:inline; margin:0px; width:110px; height:110px;">
    <img src="https://github.com/tanisharajgor/als-translation/assets/54627422/c732fb25-9bc9-4a7e-aee1-4af4a381d80d" alt="e-labelled" style="display:inline; margin:0px; width:110px; height:110px;">
</div>


## Gesture: Real-time ALS Translation & Speech

The World Health Organization (WHO) reports that more than 7% of the word’s populations has hearing impairments. An estimated 900 million people will experience hearing loss in 2050. What if there was a method to facilitate communication between sign and non-sign speakers?

### Background

Sign languages are visual representations of hand gestures, finger movements, facial expression, body movements, facial expression, body movement, etc. This structure can vary spatially and temporally.

Current state-of-the-art technologies:

Glove/Sensor Based - signer wears a pair of gloves, to capture real-time hand and finger movements, for example the Leap motion sensor.

Computer Vision Based - reads the movements of the human body, typically hand movements and uses these gestures to interpret sign language. 

With the recent advances in Mixed Reality (XR), such as the Meta Quest and Apple Vision, we propose a vision-to-speech approach, integrating recognition technologies with the real-world. Imagine features where your glasses/headsets could translate sign, you could provide further accessibility on Zoom, Teams, or FaceTime. 

### Methods

For model training, I use the large-scale [Word-Level American Sign Language (WLASL)](https://github.com/dxli94/WLASL/) video dataset, containing more than 2000 words performed by over 100 signers. To my knowledge, it is by far the largest public ASL dataset to facilitate word-level sign recognition research.

1. Sign language detection on a smaller scale - capture an image and predict what letter is being signed.
2. Transfer learning on WLASL - for each video, detect the facial and hand key-points, and then predict the word being signed.

*We primarily focus on analyzing still signing as opposed to action-based signing, which also takes into account facial expressions and semantics.

### Examples
| original_video | key_point_mapping_prediction |
|----------------|------------------------------|
| <img src="selected_gifs/65011.gif" width="400"> | <img src="selected_gifs/65011%20-%20keypoints.gif" width="400"> |
| <img src="selected_gifs/65014.gif" width="400"> | <img src="selected_gifs/65014%20-%20keypoints.gif" width="400"> |
| <img src="selected_gifs/65229.gif" width="400"> | <img src="selected_gifs/65229%20-%20keypoints.gif" width="400"> |
| <img src="selected_gifs/65374.gif" width="400"> | <img src="selected_gifs/65374%20-%20keypoints.gif" width="400"> |
| <img src="selected_gifs/65415.gif" width="400"> | <img src="selected_gifs/65415%20-%20keypoints.gif" width="400"> |
| <img src="selected_gifs/65438.gif" width="400"> | <img src="selected_gifs/65438%20-%20keypoints.gif" width="400"> |
| <img src="selected_gifs/65748.gif" width="400"> | <img src="selected_gifs/65748%20-%20keypoints.gif" width="400"> |
| <img src="selected_gifs/66123.gif" width="400"> | <img src="selected_gifs/66123%20-%20keypoints.gif" width="400"> |
| <img src="selected_gifs/66283.gif" width="400"> | <img src="selected_gifs/66283%20-%20keypoints.gif" width="400"> |
| <img src="selected_gifs/66331.gif" width="400"> | <img src="selected_gifs/66331%20-%20keypoints.gif" width="400"> |
| <img src="selected_gifs/66487.gif" width="400"> | <img src="selected_gifs/66487%20-%20keypoints.gif" width="400"> |








