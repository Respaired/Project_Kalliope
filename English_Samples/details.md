- Conformer-based style encoder
- Conformer-based duration predictor with cross attention
- Conformer-based decoder
- ConvNextV2 for the Text Encoder
- No semantic encoder right now
- Diffusion sampler Trained
- Not E2E, using [RiFornet](https://github.com/Respaired/RiFornet_Vocoder) for vocoding.
- hidden dim 1024 + 512 for Style vectors (overall 1.2B parameters, but not all of them are active at once, so training it was surprisingly affordable.)
- around 400-500 hours of data; the data is very complex & noisy. but it covers conversational, whisper, narration and wide ranges of emotions.
- signs of overfitting
- ~200K steps trained
- 44.1khz + 128 mel bins
