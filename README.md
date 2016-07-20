# Bayesian Ideal Point IRT Models in R using JAGS and Stan

*Ideal point* IRT models differ from regular IRT in that the discrimination parameter in a 2-parameter IRT model cannot be negative, whereas in an ideal point model it can. `BUGS` or `JAGS` users can find a host of regular IRT models in Ian Curtis' [paper](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=0ahUKEwjEk-b0_oLOAhUGDpAKHd4CCjMQFggeMAA&url=https%3A%2F%2Fwww.jstatsoft.org%2Farticle%2Fview%2Fv036c01%2Fv36c01.pdf&usg=AFQjCNEs9TOxtdwHK3wdInSin01WCa-Iyw&sig2=Pg9jjBeFewZIzYaAIE_gTg). Here I have included a bunch of *ideal point* IRT models, coded in Stan and JAGS for use in R. `JAGS` is commonly used in the field for this type of model, but I would recommend using Stan, as `JAGS` can take a very long time. The reason for this is that `JAGS` is unable to build a Directed Acyclic Graph from the unobserved regressor in the basic ideal point IRT equation:

![](http://i.imgur.com/gGoK7mr.png?1)
  
(see [here](https://sourceforge.net/p/mcmc-jags/discussion/610037/thread/5c9e9026/ )).

Among the models saved here are the basic IRT ideal point model, a multidimensional version, a dynamic version, and a multilevel version. Grouplet and testlet models are also included. THe basic IRT ideal point model is due to [Jackman](http://pan.oxfordjournals.org.sci-hub.cc/content/9/3/227.abstract).


