# Attentive-Snippet-Prompting-for-video-retrieval
### Demo for ASP ###
This is the implementation for the paper Attentive Snippet Prompting for Video Retrieval.

ASP is a video-text retreval pardigm based on [CLIP (ViT-B)](https://github.com/openai/CLIP) and [CLIP4Clip (ViT-B)](https://github.com/ArrowLuo/CLIP4Clip). We find that, since a video contains rich and complex content, different annotators often give divsersified texts to desribe this video, As shown below, each ground-truth text may just refer to a video snippet, and a video may contain different snippets for different text queries.

![ASP4retrieval](FrameToy1.png)

We propose a concise and novel Attentive Snippet Prompting (ASP) paradigm, which smartly leverages the text query as guidance, and attentively exploits a relevant snippet prompt from video. ASP can effectively boost video retrieval, with cooperation of such text-driven snippet prompt and global video token.
It onsists of two key modules, i.e., snippet prompting and video aggregating as shown in the following figure，

![ASP4retrieval](Frame.png)
Our ASP simply outperforms the baseline and achieved the SOTA at that time．


## Requirement
```sh
# From CLIP
conda install --yes -c pytorch pytorch=1.7.1 torchvision cudatoolkit=11.0
pip install ftfy regex tqdm
pip install opencv-python boto3 requests pandas
```
