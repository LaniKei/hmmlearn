# hmmlearn
running an example.

Following the example on the hmmlearn 0.2.1 documentation page 
https://hmmlearn.readthedocs.io/en/latest/auto_examples/plot_hmm_sampling.html#sphx-glr-auto-examples-plot-hmm-sampling-py
I have issues importing hmm from hmmlearn. Version hmmlearn 0.3.0b

First error was 
ImportError: cannot import name 'distribute_covar_matrix_to_match_covariance_type'
which I fixed, following this instructions
https://github.com/hmmlearn/hmmlearn/commit/510ae05c38ff046f00641712187b279cc498fd0a

But now I get the error

ImportError                               Traceback (most recent call last)
<ipython-input-3-16c29f744bfe> in <module>
----> 1 from hmmlearn import hmm

~\Anaconda3\lib\site-packages\hmmlearn\hmm.py in <module>
     14 from scipy.misc import logsumexp
     15 from sklearn import cluster
---> 16 from sklearn.mixture import _validate_covars
     17 from sklearn.utils import check_random_state
     18 

ImportError: cannot import name '_validate_covars'


which is also located at sklearn.mixture, just like the error before.
Can I do something to fix the sklearn.mixture problem?
I already uninstalled and reinstalled scikit-learn.
Or:
Where can I find hmmlearn 0.3.0b examples which work in order to learn about how to use hmmlearn?
