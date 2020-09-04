## [Predicting the Success Rate of Video Ads](https://github.com/buseOzr/PredictingtheSuccessRate)

This master’s thesis is written in cooperation between Smart AdServer’s Research and
Development Department and CentraleSupelec.You can access the master thesis report and the presentation through the link above.

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

* There is no trend in AUC over time
  * Run experiments on multiple days
* XGBoost model outperforms Decision Tree, AdaBoost and Random Forest
 * Better AUC, better control over the model
 * Scalable and parallelizable
* High variance in data	
 * The model has to be adaptive and flexible rather than assigning fixed parameters
 * Early Stopping mechanism
* XGBoost and Neural Network performs nearly the same
 * Neural Network requires more expertise
* Implementation of Neural Network has some advantages
 * Continuous Learning
 * Serving in production
 * Transfer Learning



