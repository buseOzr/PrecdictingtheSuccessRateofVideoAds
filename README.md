## [Predicting the Success Rate of Video Ads](https://github.com/buseOzr/PredictingtheSuccessRate)

This master’s thesis is written in cooperation between Smart AdServer’s Research and
Development Department and CentraleSupelec. The master thesis report and the presentation are accessible through the link above.

### Abstract
With the extensive usage of video ads in the digital advertising industry,
achieving a high success rate of video-based advertisements has gained significant importance
in the ad tech industry. Hence it is essential to deliver video advertisements to end-users
seamlessly. SSPs need to choose the best advertiser per auction whose ads can
be delivered without having problems on the corresponding publisher’s website. These
problems could be raised due to time-out, internet connection problem, non-compliant
video format, and incompatibility between publishers and advertisers.
However, ad tech companies want to prevent this obstacle in order to serve the best
experience to end-users, to give substantial benefit to advertisers, to increase the revenue
of publishers and the regarding ad server company because if an ad is served on the serverside,
though it fails on the client-side, it is not exposed to an end-user. Consequently,
there is no revenue either for a publisher or an ad server. Moreover, the advertiser is not
able to show its content to a user. This situation is undesirable for all parties. __Therefore
this study proposes a methodology that builds a machine learning model in order to
predict the success rate of video ads for given constraints, compare the state-of-the-art approaches and improve them progressively__
. This method helps SSPs to calculate the expected revenue of each bidder in an auction. By doing so, the ad server
chooses a bidder with the highest expected revenue. Consequently, SSPs can
increase the success/delivery rate of video ads and its revenue.

### Conclusion

In summary, this study discusses different state-of-the-art approaches in order to predict
the delivery rate/success rate of video ads. An iterative approach is followed throughout
the study. At each step, some changes are applied, and their impact is analyzed on
the corresponding model. First of all, different tree-based models are compared, and
the best performing algorithm is chosen for further improvements. As a result, Extreme
Gradient Boosting gives clearly better results than Decision Tree, Ada Boost, and Random
Forest. Besides performing well, Extreme Gradient Boosting is scalable and parallelizable.
Although it is harder to tune it compared to the other tree-based classifiers due to the
high number of parameters, it allows us to have more control over the model.
During the experiments, it is realized that there is a high variation in data, and the
distribution changes over time. Therefore, the model should be adaptive and flexible,
depending on the data set of any given time in order to perform well. Consequently, the
parameters of the model should not be the same; thus, early stopping strategy is applied
in order to adapt the changes over time. Furthermore, due to the data variance in time,
the model should be trained with the most current data as frequently as possible in order
to get the greatest performance.
Moreover, Extreme Gradient Boosting and Neural Network models are trained to
compare their results and analyze their advantages and disadvantages. In conclusion,
even though their results are very similar to each other, Extreme Gradient Boosting performs
slightly better than the Neural Network model. However, it is difficult to reach a
conclusion since there is a slight difference between the two models. Moreover, there are a few advantages
of using neural networks over XGBoost as follows. As a reminder, TensorFlow is
used to implement the Neural Network model in the study. TensorFlow
provides the flexibility of building a better pipeline, the stable solution for serving in production,
and the possibility for transfer learning for future projects. Another advantage
is the ability to apply continuous learning, which is progressive and adaptive as new data
is acquired. These advantages make the neural network more suitable. 
