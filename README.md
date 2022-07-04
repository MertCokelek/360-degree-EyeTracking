# 360-degree-EyeTracking

## Collecting Eye-Tracking Data 
- See [Google Doc.](https://docs.google.com/document/d/1BiEkwVO8YIm0r21k1gQBSp9t3gLNPU6T_AB2RDecotY/edit?usp=sharing)


## Ambisonic Plugin for Unity
1. Download and extract the `unitypackage` from: https://github.com/Professor3DSound/Vive3DSP

    **The following steps are adapted from [here](https://hub.vive.com/storage/3dsp/vive_3dsp_audio_sdk_unity_plugin.html)**

2. Create a new 3D project, or, open an existing project.
3. Click **Assets > Import Package > Custom Package**
4. Select `Vive3DSP_v1.2.8.0`, select all and click **Import**.
5. In Unity, click **Edit > Project Settings > Audio**.
    - Select **VIVE 3DSP Spatializer** in **Spatializer Plugin** and **Ambisonic Decoder Plugin**
6. Right click on Unity Asset Window, **Import New Asset**, select an ambisonic audio file.
    - Example [**audio**](https://drive.google.com/file/d/1-HY7ls1X5XtCcwe4cOp-vREpljt8xjJ8/view?usp=sharing) and its [**video**](https://drive.google.com/file/d/1-G0_L76Cbd83tXCJDpGZjl5AUy4TROx9/view?usp=sharing) are here.
    - The audio should be in: **_4-channel B-format_**. **_(ACN/SN3D)_**
7. Right click on Unity Project Hierarchy, add new audio source: **Audio > Audio Source**.
    - In the inspector tab, select the imported audio asset in `AudioClip`
    - Make sure `Spatialize` is **not** selected.
8. Play the scene to test.
