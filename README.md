# Text-to-Speech and Audiobook Creation with ML Models

(!) Please note: this TTS machine-learning project used the LJSpeech dataset, which is available open-source online and would need to be downloaded, in order to replicate this data science project.

## Introduction

In this project, we set out to explore the creation of text-to-speech (TTS) audiobooks and application of machine learning. Our goal was to learn about the use of AI in audiobook creation, and see how we could deploy and improve our machine learning skills in the creation of a TTS model. In the model training phase, we used the LJSpeech dataset.

## Methodology

### Initial Training

We started the project with a pre-made notebook for training the TTS model, but quickly realized that training parameters needed to be changed/optimized to avoid endless training time. The learning curve was large and the machine learning model code diverged significantly at points from familiar Python code.

There were difficulties with TensorBoard, which would have made the training process more transparent if it had worked, and the information overload was significant with numerous new model features, error identification and model iterations. We had to make this crucial adjustment to streamline the training process and accelerate our machine learning experiments.

### Experimentation with Simple Models

Now we made a significant and historic achievement - the creation of a basic TTS model through minimal training (only a few minutes duration with 10 epochs), colloquially referred to as a "fart box". This experiment demonstrated the feasibility of quickly prototyping TTS systems with limited training data, but the outcome was far from desired.  

### Transition to Pre-Trained Models

At this point, we had an improved though still rudimentary understanding of TTS technology, and with expert advice transitioned to exploring and deploying pre-trained TTS models. This shift allowed us to benefit from existing (and reliably effective) resources, which massively accelerated the development process. Moreover, it enabled us to focus on fine-tuning specific aspects of the models, as opposed to starting from scratch each time with the creation of a new TTS model.

### Local Training Exploration

We wanted to have more control over the training process, and experimented with using command-line interfaces to ‘fit’ pre-trained models, such as Tacotron2 and xtts_v2, to desired text. Although this approach provided greater autonomy, we encountered challenges, namely computer crashes during the final stages of clip generation. Despite these setbacks, we were eventually able to generate reliable and very comprehensible (if not extremely precise) audio from various texts. this exploration enhanced my comprehension of TTS model architecture and optimization techniques.

### Utilization of Colab for Training

Throughout this project, we were using Google Colab (initially basing our code on the CoquiTTS tutorial) and we continued this when listing, selecting, and training the various pre-trained models that are available open-source. Colab definitely offers advantages in terms of computational resources and ease of use. Workflow efficiency was mostly improved and the user interface was helpful at times when the information overload and learning curve threatened to overwhelm.


### Performance Evaluation

Through experimentation, it was discovered that the training time for TTS models with basic GPU resources averaged approximately 1.6 times the playback time of the resulting clips. This was valuable insight for the creation of future TTS resources, especially when estimating resource requirements and optimizing training schedules.

### Fine-Tuning Focus

An important observation was the significance of fine-tuning sentence endings, as they often required adjustments to enhance naturalness and coherence in generated speech. This insight guided future iterations and refinements in model training and optimization.

## Results

The culmination of these efforts yielded a 10-minute TTS clip, representing the most successful outcome of the project thus far. We also managed to clone (although not to a very accurate extent) our voices and use them to generate speech from inputted text. This was a very enjoyable aspect of the project and rewarded our perseverance to better understand and deploy TTS models. Not only this, but by “leveraging” pre-trained models and using smarter model-training strategies, we observed notable improvements in TTS performance and efficiency.

## Conclusion

In conclusion, this project served as a comprehensive exploration of TTS technology, from initial training endeavors to advanced optimization, and offered a sneak peek into the application of machine learning to develop quick and precise speech-generation. Ultimately, we learned (but definitely did not master) how to create and train a basic TTS model using an existing dataset. This was a rewarding process, but for any future projects that involve TTS, such as the creation of a full audiobook, we will probably opt to use pre-trained models and spend the significant volume of time saved to fine-tune parameters and tinker with the final product - in particular to remove the long gaps at the end of sentences!
