# Content-based Video Relevance Prediction Challenge
### @ACM Multimedia 2018, Seoul, South Korea

(This challenge is fully sponsored by Hulu.)

Video relevance computation is one of the most important tasks for personalized online streaming service. Given the relevance of videos and viewer feedbacks, the system can provide personalized recommendations, which will help the viewer discover more content of interest. In most online service, the computation of video relevance table is based on the viewers' implicit feedback, e.g. watch and search history. The system analyzes the viewer-to-video preference and computes the video-to-video relevance scores using collaborative filtering based methods. However, this kind of method performs poorly for “cold-start” problems - when a new video is added to the library, the recommendation system needs to bootstrap the video relevance score with very little historical viewer feedbacks. One promising approach to solve “cold-start” is analyzing video content itself to predict the relevance score, i.e. predicting the video-to-video relevance by analyzing the keyframes, audio, subtitles and metadata. With the relevance score, we can provide better recommendations for our viewers.

## Task and Data

The main task of this challenge is to predict the relevance between TV-shows or movies from video content and its features. Specifically, there are two separated tracks for TV-shows and movies respectively. The following components will be publicly available under this challenge:

#### Track 1: TV-shows

Pre-extracted features derived from nearly 7,000 TV-show video trailers. The whole set is divided into 3 subsets: training set (3,000 shows), validation set (over 800 shows), and testing set (3,000 shows).

#### Track 2: Movies

Pre-extracted features derived from over 10,000 movie video trailers. The whole set is divided into 3 subsets: training set (4,500 movies), validation set (over 1000 movies), and testing set (4,500 movies).

For training set and validation set in both tracks, we also provide the ground truth (relevance lists) derived from implicit viewer feedbacks. The viewer feedbacks have been cleaned to avoid any privacy issues.

The proposed methods will be evaluated based on recall rate regarding to top K prediction (the value of K is 100 as the final criteria). We will provide the python script to compute recall for evaluation.

## Citation

If you use the CBVRP dataset in your work, please cite it as

Mengyi Liu, Xiaohui Xie, Hanning Zhou. "Content-based Video Relevance Prediction Challenge: Data, Protocol, and Baseline". arXiv preprint arXiv:1806.00737. 2018.
"README.md" 73L, 4951C
