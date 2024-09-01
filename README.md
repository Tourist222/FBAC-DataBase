# FBAC-DataBase
**Chinese Multimodal Emotion Database Based on Facial Expressions, Body Movements, and Sounds (FBAC-DB)**

The purpose of this dataset is to enhance the joint study of the interrelationships between facial expressions, acoustic information, and body movements when expressing emotions. We have learned that the movement of limbs and bones is one of the most universal and complex ways of communication for humans, with numerous functions, as evidenced by the number of disciplines involved. In previous studies, workers mainly focused on facial, vocal, and textual aspects in emotional expression and perception. In recent studies, body movements and posture changes have been shown to convey specific information about a person's emotions, particularly in terms of whole-body movement, arm movements, and posture. Therefore, we use deep sensing lenses to detect depth information, enhance bone recognition, and capture motion.

<img src="Images/show.jpg#pic_center" width="80%" ></img>

<img src="Images/picture.png#pic_center" width="85%" ></img>

## 1 Dataset Design

### 1.1 emotional category

This dataset is designed as a discrete emotion model, which adds the category of "neutral" as a control emotion on the basis of six basic emotions. The seven emotions are neutral, happy, sad, angry, disgusted, surprised, and scared.

### 1.2 emotional stimulation

Unlike most emotion datasets, this dataset uses performance and elicitation to elicit specific emotions from participants. We have designed two triggering methods. The first method is to construct corresponding short virtual scenes for participants of different emotional categories. The second method is to provide real sample materials including pictures, audio, and videos to stimulate participants to express their corresponding emotions.

### 1.3 collection object

This data focuses on acoustic information, so the influence of regional differences can be ignored. During the recording process,
We recruited 100 volunteers from within the school, mainly consisting of students aged 18 to 30. Excluding 20 volunteers with poor expression effects, 80 participants were ultimately selected for recording. These participants are all physically healthy, without any mental illness or psychological disorders.

### 1.4 expression content

When selecting speech text content, we referred to the standards of EMO-DB dataset and CASIA Chinese sentiment corpus, striving to make the corpus text semantically neutral and devoid of emotional tendencies, in order to truly reflect the emotional changes in speech. The text content should be close to the style of daily spoken language and avoid excessive modifications in written language.

<img src="Images/contents.png#pic_center" width="80%" ></img>

## 2 Data Collection

### 2.1 data collection

We have set up and constructed a specialized audio and video data collection environment. Due to changes in indoor lighting over time, the brightness of video footage captured at different time periods varies significantly. To ensure the stability of lighting conditions, we have added two professional grade fill lights.

<img src="Images/environment.jpg#pic_center" width="50%" ></img>

### 2.2 collection process

For each emotion, participants are required to start expressing their emotions in a neutral emotional state, with their hands naturally flat on the table and their facial expressions facing the camera naturally; After the participants showed facial expressions, upper body movements, and speech, they put their hands back on the table and their expressions returned to their natural state. This is a complete expression process that every data sample must have. After exhibiting a specific emotional category, participants are required to wait at least 3 seconds before expressing their emotions again.

## 3 Data Organization

### 3.1 data Editing

Different editing strategies were adopted for emotions with different speech rates. For fast-paced emotions such as happiness and anger, the video duration is set to about 4 seconds to 5 seconds; For sad emotions with slower speaking speed, the duration is adjusted to about 7 seconds. After editing, each shot produced an average of 10438 video clips, with a total memory usage of approximately 110GB. Finally, these edited videos were converted into WAV format audio using Wanxing Youzhuan software for subsequent analysis work.

<img src="Images/show_one.jpg#pic_center" width="70%" ></img>


### 3.2 data distribution

For the positive perspective, a total of 5106 samples were generated, with only one neutral performance, so the sample size is relatively small. The small number of happy and surprised samples may be due to previous data editing and difficulty in performance, while the rest of the classification samples are relatively balanced. 

<img src="Images/distribution.jpg#pic_center" width="50%" ></img>

## When to upload

*Samples of this dataset will be upload before 2025 (After the related work is published)*
